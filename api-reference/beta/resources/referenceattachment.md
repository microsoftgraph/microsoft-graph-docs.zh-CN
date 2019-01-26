---
title: referenceAttachment 资源类型
description: '指向文件夹或文件 （如文本文件或 Word 文档中） 上的 OneDrive for Business 云驱动器或其他受支持的存储位置，附加到的链接 '
localization_priority: Normal
ms.openlocfilehash: adf078f7ba678a4fe90a51972c5e4be4788c9c0c
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574556"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="7794c-103">referenceAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="7794c-103">referenceAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7794c-104">链接到的文件夹或文件 （如文本文件或 Word 文档中） 上 OneDrive for Business 云驱动器或其他支持的存储位置，附加到[事件](../resources/event.md)、[消息](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[发布](../resources/post.md)。</span><span class="sxs-lookup"><span data-stu-id="7794c-104">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="7794c-105">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="7794c-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="7794c-106">方法</span><span class="sxs-lookup"><span data-stu-id="7794c-106">Methods</span></span>

| <span data-ttu-id="7794c-107">方法</span><span class="sxs-lookup"><span data-stu-id="7794c-107">Method</span></span>       | <span data-ttu-id="7794c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="7794c-108">Return Type</span></span>  |<span data-ttu-id="7794c-109">说明</span><span class="sxs-lookup"><span data-stu-id="7794c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7794c-110">Get</span><span class="sxs-lookup"><span data-stu-id="7794c-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="7794c-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="7794c-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="7794c-112">读取 referenceAttachment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7794c-112">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="7794c-113">删除</span><span class="sxs-lookup"><span data-stu-id="7794c-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="7794c-114">无</span><span class="sxs-lookup"><span data-stu-id="7794c-114">None</span></span> |<span data-ttu-id="7794c-115">删除 referenceAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="7794c-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="7794c-116">属性</span><span class="sxs-lookup"><span data-stu-id="7794c-116">Properties</span></span>
| <span data-ttu-id="7794c-117">属性</span><span class="sxs-lookup"><span data-stu-id="7794c-117">Property</span></span>     | <span data-ttu-id="7794c-118">类型</span><span class="sxs-lookup"><span data-stu-id="7794c-118">Type</span></span>   |<span data-ttu-id="7794c-119">说明</span><span class="sxs-lookup"><span data-stu-id="7794c-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7794c-120">contentType</span><span class="sxs-lookup"><span data-stu-id="7794c-120">contentType</span></span>|<span data-ttu-id="7794c-121">String</span><span class="sxs-lookup"><span data-stu-id="7794c-121">String</span></span>|<span data-ttu-id="7794c-122">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="7794c-122">The content type of the attachment.</span></span> <span data-ttu-id="7794c-123">可选。</span><span class="sxs-lookup"><span data-stu-id="7794c-123">Optional.</span></span>|
|<span data-ttu-id="7794c-124">id</span><span class="sxs-lookup"><span data-stu-id="7794c-124">id</span></span>|<span data-ttu-id="7794c-125">String</span><span class="sxs-lookup"><span data-stu-id="7794c-125">String</span></span>|<span data-ttu-id="7794c-p102">附件 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="7794c-p102">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="7794c-128">isFolder</span><span class="sxs-lookup"><span data-stu-id="7794c-128">isFolder</span></span>|<span data-ttu-id="7794c-129">布尔值</span><span class="sxs-lookup"><span data-stu-id="7794c-129">Boolean</span></span>|<span data-ttu-id="7794c-130">指定附件是否链接到的文件夹。</span><span class="sxs-lookup"><span data-stu-id="7794c-130">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="7794c-131">必须将其设置为 true 如果**sourceUrl**文件夹的链接。</span><span class="sxs-lookup"><span data-stu-id="7794c-131">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="7794c-132">可选。</span><span class="sxs-lookup"><span data-stu-id="7794c-132">Optional.</span></span>|
|<span data-ttu-id="7794c-133">isInline</span><span class="sxs-lookup"><span data-stu-id="7794c-133">isInline</span></span>|<span data-ttu-id="7794c-134">布尔</span><span class="sxs-lookup"><span data-stu-id="7794c-134">Boolean</span></span>|<span data-ttu-id="7794c-135">如果附件显示为内嵌在嵌入对象的正文中，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="7794c-135">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="7794c-136">可选。</span><span class="sxs-lookup"><span data-stu-id="7794c-136">Optional.</span></span>|
|<span data-ttu-id="7794c-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7794c-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7794c-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7794c-138">DateTimeOffset</span></span>|<span data-ttu-id="7794c-139">上次修改附件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="7794c-139">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="7794c-140">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="7794c-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7794c-141">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="7794c-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="7794c-142">可选。</span><span class="sxs-lookup"><span data-stu-id="7794c-142">Optional.</span></span>|
|<span data-ttu-id="7794c-143">name</span><span class="sxs-lookup"><span data-stu-id="7794c-143">name</span></span>|<span data-ttu-id="7794c-144">String</span><span class="sxs-lookup"><span data-stu-id="7794c-144">String</span></span>|<span data-ttu-id="7794c-145">表示嵌入的附件的图标下面显示的文本。</span><span class="sxs-lookup"><span data-stu-id="7794c-145">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="7794c-146">这不需要是实际的文件名称。</span><span class="sxs-lookup"><span data-stu-id="7794c-146">This does not need to be the actual file name.</span></span> <span data-ttu-id="7794c-147">必需。</span><span class="sxs-lookup"><span data-stu-id="7794c-147">Required.</span></span>|
|<span data-ttu-id="7794c-148">权限</span><span class="sxs-lookup"><span data-stu-id="7794c-148">permission</span></span>|<span data-ttu-id="7794c-149">referenceAttachmentPermission</span><span class="sxs-lookup"><span data-stu-id="7794c-149">referenceAttachmentPermission</span></span>|<span data-ttu-id="7794c-150">指定**提供程序类型**中的提供程序的类型为附件授予的权限。</span><span class="sxs-lookup"><span data-stu-id="7794c-150">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="7794c-151">可取值为：`other`、`view`、`edit`、`anonymousView`、`anonymousEdit`、`organizationView`、`organizationEdit`。</span><span class="sxs-lookup"><span data-stu-id="7794c-151">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="7794c-152">可选。</span><span class="sxs-lookup"><span data-stu-id="7794c-152">Optional.</span></span>|
|<span data-ttu-id="7794c-153">previewUrl</span><span class="sxs-lookup"><span data-stu-id="7794c-153">previewUrl</span></span>|<span data-ttu-id="7794c-154">String</span><span class="sxs-lookup"><span data-stu-id="7794c-154">String</span></span>|<span data-ttu-id="7794c-155">适用于仅图像-要获取的预览图像 URL 的参考附件。</span><span class="sxs-lookup"><span data-stu-id="7794c-155">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="7794c-156">仅当**sourceUrl**标识的图像文件，请使用**thumbnailUrl**和**previewUrl** 。</span><span class="sxs-lookup"><span data-stu-id="7794c-156">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="7794c-157">可选。</span><span class="sxs-lookup"><span data-stu-id="7794c-157">Optional.</span></span>|
|<span data-ttu-id="7794c-158">提供程序类型</span><span class="sxs-lookup"><span data-stu-id="7794c-158">providerType</span></span>| <span data-ttu-id="7794c-159">referenceAttachmentProvider</span><span class="sxs-lookup"><span data-stu-id="7794c-159">referenceAttachmentProvider</span></span> |<span data-ttu-id="7794c-160">支持此 contentType 的附件的提供程序的类型。</span><span class="sxs-lookup"><span data-stu-id="7794c-160">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="7794c-161">可取值为：`other`、`oneDriveBusiness`、`oneDriveConsumer`、`dropbox`。</span><span class="sxs-lookup"><span data-stu-id="7794c-161">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="7794c-162">可选。</span><span class="sxs-lookup"><span data-stu-id="7794c-162">Optional.</span></span>|
|<span data-ttu-id="7794c-163">size</span><span class="sxs-lookup"><span data-stu-id="7794c-163">size</span></span>|<span data-ttu-id="7794c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="7794c-164">Int32</span></span>|<span data-ttu-id="7794c-165">存储在引用附件的邮件的元数据以字节为单位的大小。</span><span class="sxs-lookup"><span data-stu-id="7794c-165">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="7794c-166">此值不表示实际文件的大小。</span><span class="sxs-lookup"><span data-stu-id="7794c-166">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="7794c-167">可选。</span><span class="sxs-lookup"><span data-stu-id="7794c-167">Optional.</span></span>|
|<span data-ttu-id="7794c-168">sourceUrl</span><span class="sxs-lookup"><span data-stu-id="7794c-168">sourceUrl</span></span>|<span data-ttu-id="7794c-169">String</span><span class="sxs-lookup"><span data-stu-id="7794c-169">String</span></span>|<span data-ttu-id="7794c-170">若要获取附件内容的 URL。</span><span class="sxs-lookup"><span data-stu-id="7794c-170">URL to get the attachment content.</span></span> <span data-ttu-id="7794c-171">如果这是指向文件夹的 URL，然后为文件夹以在 Outlook 或 Outlook web 上的中正确显示设置**isFolder**为 true。</span><span class="sxs-lookup"><span data-stu-id="7794c-171">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="7794c-172">必需。</span><span class="sxs-lookup"><span data-stu-id="7794c-172">Required.</span></span>|
|<span data-ttu-id="7794c-173">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="7794c-173">thumbnailUrl</span></span>|<span data-ttu-id="7794c-174">String</span><span class="sxs-lookup"><span data-stu-id="7794c-174">String</span></span>|<span data-ttu-id="7794c-175">适用于仅图像-要获取的缩略图图像 URL 的参考附件。</span><span class="sxs-lookup"><span data-stu-id="7794c-175">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="7794c-176">仅当**sourceUrl**标识的图像文件，请使用**thumbnailUrl**和**previewUrl** 。</span><span class="sxs-lookup"><span data-stu-id="7794c-176">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="7794c-177">可选。</span><span class="sxs-lookup"><span data-stu-id="7794c-177">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7794c-178">关系</span><span class="sxs-lookup"><span data-stu-id="7794c-178">Relationships</span></span>
<span data-ttu-id="7794c-179">无</span><span class="sxs-lookup"><span data-stu-id="7794c-179">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="7794c-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7794c-180">JSON representation</span></span>

<span data-ttu-id="7794c-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7794c-181">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.referenceAttachment"
}-->

```json
{
  "contentType": "string",
  "id": "string (identifier)",
  "isFolder": true,
  "isInline": true,
  "lastModifiedDateTime": "String (timestamp)",
  "name": "string",
  "permission": "referenceAttachmentPermission",
  "previewUrl": "string",
  "providerType": "referenceAttachmentProvider",
  "size": 1024,
  "sourceUrl": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/referenceattachment.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
