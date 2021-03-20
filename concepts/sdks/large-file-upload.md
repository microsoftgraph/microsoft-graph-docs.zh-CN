---
title: 使用 Microsoft Graph SDK 上载大文件
description: 提供有关使用 Microsoft Graph SDK 上载大文件的指南。
localization_priority: Normal
author: DarrelMiller
ms.openlocfilehash: 54ff14071a81ac286cebbd785216c02dc9cf6c23
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948635"
---
# <a name="upload-large-files-using-the-microsoft-graph-sdks"></a><span data-ttu-id="bfa5b-103">使用 Microsoft Graph SDK 上载大文件</span><span class="sxs-lookup"><span data-stu-id="bfa5b-103">Upload large files using the Microsoft Graph SDKs</span></span>

<span data-ttu-id="bfa5b-104">Microsoft Graph 中的许多实体支持可 [恢复文件上载](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0&preserve-view=true) ，以便更轻松地上载大文件。</span><span class="sxs-lookup"><span data-stu-id="bfa5b-104">A number of entities in Microsoft Graph support [resumable file uploads](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0&preserve-view=true) to make it easier to upload large files.</span></span> <span data-ttu-id="bfa5b-105">文件被切片为较小的片段，并且请求用于上载单个切片，而不是尝试在单个请求中上载整个文件。</span><span class="sxs-lookup"><span data-stu-id="bfa5b-105">Instead of trying to upload the entire file in a single request, the file is sliced into smaller pieces and a request is used to upload a single slice.</span></span> <span data-ttu-id="bfa5b-106">为了简化此过程，Microsoft Graph SDK 实现了管理切片上载的大型文件上载任务。</span><span class="sxs-lookup"><span data-stu-id="bfa5b-106">In order to simplify this process, the Microsoft Graph SDKs implement a large file upload task that manages the uploading of the slices.</span></span>

## <a name="c"></a>[<span data-ttu-id="bfa5b-107">C#</span><span class="sxs-lookup"><span data-stu-id="bfa5b-107">C#</span></span>](#tab/csharp)

```csharp
using (var fileStream = System.IO.File.OpenRead(filePath))
{
    // Use properties to specify the conflict behavior
    // in this case, replace
    var uploadProps = new DriveItemUploadableProperties
    {
        ODataType = null,
        AdditionalData = new Dictionary<string, object>
        {
            { "@microsoft.graph.conflictBehavior", "replace" }
        }
    };

    // Create the upload session
    // itemPath does not need to be a path to an existing item
    var uploadSession = await graphClient.Me.Drive.Root
        .ItemWithPath(itemPath)
        .CreateUploadSession(uploadProps)
        .Request()
        .PostAsync();

    // Max slice size must be a multiple of 320 KiB
    int maxSliceSize = 320 * 1024;
    var fileUploadTask =
        new LargeFileUploadTask<DriveItem>(uploadSession, fileStream, maxSliceSize);

    // Create a callback that is invoked after each slice is uploaded
    IProgress<long> progress = new Progress<long>(prog => {
        Console.WriteLine($"Uploaded {prog} bytes of {fileStream.Length} bytes");
    });

    try
    {
        // Upload the file
        var uploadResult = await fileUploadTask.UploadAsync(progress);

        if (uploadResult.UploadSucceeded)
        {
            // The ItemResponse object in the result represents the
            // created item.
            Console.WriteLine($"Upload complete, item ID: {uploadResult.ItemResponse.Id}");
        }
        else
        {
            Console.WriteLine("Upload failed");
        }
    }
    catch (ServiceException ex)
    {
        Console.WriteLine($"Error uploading: {ex.ToString()}");
    }
}
```

## <a name="typescript"></a>[<span data-ttu-id="bfa5b-108">TypeScript</span><span class="sxs-lookup"><span data-stu-id="bfa5b-108">TypeScript</span></span>](#tab/typescript)

```typescript
const options: any = {
    // Relative path from root to destination folder
    path: itemPath,
    // file is a File object, typically from an <input type="file"/>
    fileName: file.name,
    rangeSize: 320 * 1024
  }

  try {
    const uploadTask: MicrosoftGraph.OneDriveLargeFileUploadTask =
      await MicrosoftGraph.OneDriveLargeFileUploadTask.create(client, file, options);

    const uploadedFile: DriveItem = await uploadTask.upload();

    console.log(JSON.stringify(`Uploaded file with ID: ${uploadedFile.id}`));
    return `Uploaded file with ID: ${uploadedFile.id}`;
  } catch (err) {
    console.log(`Error uploading file: ${JSON.stringify(err)}`);
    return `Error uploading file: ${JSON.stringify(err)}`;
  }
}
```

## <a name="java"></a>[<span data-ttu-id="bfa5b-109">Java</span><span class="sxs-lookup"><span data-stu-id="bfa5b-109">Java</span></span>](#tab/java)

```java
// Get an input stream for the file
File file = new File(localFilePath);
InputStream fileStream = new FileInputStream(file);
long streamSize = file.length();

// Create a callback used by the upload provider
IProgressCallback<DriveItem> callback = new IProgressCallback<DriveItem>() {
    @Override
    // Called after each slice of the file is uploaded
    public void progress(final long current, final long max) {
        System.out.println(
            String.format("Uploaded %d bytes of %d total bytes", current, max)
        );
    }
};

// Create an upload session
UploadSession uploadSession = graphClient
    .me()
    .drive()
    .root()
    // itemPath like "/Folder/file.txt"
    // does not need to be a path to an existing item
    .itemWithPath(itemPath)
    .createUploadSession(new DriveItemUploadableProperties())
    .buildRequest()
    .post();

LargeFileUploadTask<DriveItem> largeFileUploadTask =
    new LargeFileUploadTask<DriveItem>
        (uploadSession, graphClient, fileStream, streamSize, DriveItem.class);

// Config parameter is an array of integers
// customConfig[0] indicates the max slice size
// Max slice size must be a multiple of 320 KiB
int[] customConfig = { 320 * 1024 };

// Do the upload
largeFileUploadTask.upload(callback, customConfig);
```

---

## <a name="resuming-a-file-upload"></a><span data-ttu-id="bfa5b-110">恢复文件上载</span><span class="sxs-lookup"><span data-stu-id="bfa5b-110">Resuming a file upload</span></span>

<span data-ttu-id="bfa5b-111">Microsoft Graph SDK 支持 [恢复进行中的上传](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0&preserve-view=true#resuming-an-in-progress-upload)。</span><span class="sxs-lookup"><span data-stu-id="bfa5b-111">The Microsoft Graph SDKs support [resuming in-progress uploads](/graph/api/driveitem-createuploadsession?view=graph-rest-1.0&preserve-view=true#resuming-an-in-progress-upload).</span></span> <span data-ttu-id="bfa5b-112">如果应用程序在上载过程中遇到连接中断或 5.x.x HTTP 状态，您可以继续上载。</span><span class="sxs-lookup"><span data-stu-id="bfa5b-112">If your application encounters a connection interruption or a 5.x.x HTTP status during upload, you can resume the upload.</span></span>

<!-- markdownlint-disable MD024 -->
### <a name="c"></a>[<span data-ttu-id="bfa5b-113">C#</span><span class="sxs-lookup"><span data-stu-id="bfa5b-113">C#</span></span>](#tab/csharp)

```csharp
fileUploadTask.ResumeAsync(progress);
```

### <a name="typescript"></a>[<span data-ttu-id="bfa5b-114">TypeScript</span><span class="sxs-lookup"><span data-stu-id="bfa5b-114">TypeScript</span></span>](#tab/typescript)

```typescript
const resumedFile: DriveItem = await uploadTask.resume();
```

### <a name="java"></a>[<span data-ttu-id="bfa5b-115">Java</span><span class="sxs-lookup"><span data-stu-id="bfa5b-115">Java</span></span>](#tab/java)

> [!NOTE]
> <span data-ttu-id="bfa5b-116">当前Java SDK 不支持恢复进行中的下载。</span><span class="sxs-lookup"><span data-stu-id="bfa5b-116">The Java SDK does not currently support resuming in-progress downloads.</span></span>

---
<!-- markdownlint-enable MD024 -->
