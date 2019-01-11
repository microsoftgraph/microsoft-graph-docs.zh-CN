---
title: referenceAttachment 资源类型
description: '指向文件夹或文件 （如文本文件或 Word 文档中） 上的 OneDrive for Business 云驱动器或其他受支持的存储位置，附加到的链接 '
localization_priority: Normal
ms.openlocfilehash: 6a334b303bea7aff768733434b9ba882de237a12
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27880050"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="ae341-103">referenceAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="ae341-103">referenceAttachment resource type</span></span>

> <span data-ttu-id="ae341-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ae341-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae341-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ae341-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ae341-106">链接到的文件夹或文件 （如文本文件或 Word 文档中） 上 OneDrive for Business 云驱动器或其他支持的存储位置，附加到[事件](../resources/event.md)、[消息](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[发布](../resources/post.md)。</span><span class="sxs-lookup"><span data-stu-id="ae341-106">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="ae341-107">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="ae341-107">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="ae341-108">方法</span><span class="sxs-lookup"><span data-stu-id="ae341-108">Methods</span></span>

| <span data-ttu-id="ae341-109">方法</span><span class="sxs-lookup"><span data-stu-id="ae341-109">Method</span></span>       | <span data-ttu-id="ae341-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ae341-110">Return Type</span></span>  |<span data-ttu-id="ae341-111">说明</span><span class="sxs-lookup"><span data-stu-id="ae341-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ae341-112">Get</span><span class="sxs-lookup"><span data-stu-id="ae341-112">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="ae341-113">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="ae341-113">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="ae341-114">读取 referenceAttachment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ae341-114">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="ae341-115">删除</span><span class="sxs-lookup"><span data-stu-id="ae341-115">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="ae341-116">无</span><span class="sxs-lookup"><span data-stu-id="ae341-116">None</span></span> |<span data-ttu-id="ae341-117">删除 referenceAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="ae341-117">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ae341-118">属性</span><span class="sxs-lookup"><span data-stu-id="ae341-118">Properties</span></span>
| <span data-ttu-id="ae341-119">属性</span><span class="sxs-lookup"><span data-stu-id="ae341-119">Property</span></span>     | <span data-ttu-id="ae341-120">类型</span><span class="sxs-lookup"><span data-stu-id="ae341-120">Type</span></span>   |<span data-ttu-id="ae341-121">说明</span><span class="sxs-lookup"><span data-stu-id="ae341-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae341-122">contentType</span><span class="sxs-lookup"><span data-stu-id="ae341-122">contentType</span></span>|<span data-ttu-id="ae341-123">String</span><span class="sxs-lookup"><span data-stu-id="ae341-123">String</span></span>|<span data-ttu-id="ae341-124">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="ae341-124">The content type of the attachment.</span></span> <span data-ttu-id="ae341-125">可选。</span><span class="sxs-lookup"><span data-stu-id="ae341-125">Optional.</span></span>|
|<span data-ttu-id="ae341-126">id</span><span class="sxs-lookup"><span data-stu-id="ae341-126">id</span></span>|<span data-ttu-id="ae341-127">String</span><span class="sxs-lookup"><span data-stu-id="ae341-127">String</span></span>|<span data-ttu-id="ae341-p103">附件 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="ae341-p103">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="ae341-130">isFolder</span><span class="sxs-lookup"><span data-stu-id="ae341-130">isFolder</span></span>|<span data-ttu-id="ae341-131">布尔</span><span class="sxs-lookup"><span data-stu-id="ae341-131">Boolean</span></span>|<span data-ttu-id="ae341-132">指定附件是否链接到的文件夹。</span><span class="sxs-lookup"><span data-stu-id="ae341-132">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="ae341-133">必须将其设置为 true 如果**sourceUrl**文件夹的链接。</span><span class="sxs-lookup"><span data-stu-id="ae341-133">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="ae341-134">可选。</span><span class="sxs-lookup"><span data-stu-id="ae341-134">Optional.</span></span>|
|<span data-ttu-id="ae341-135">isInline</span><span class="sxs-lookup"><span data-stu-id="ae341-135">isInline</span></span>|<span data-ttu-id="ae341-136">布尔</span><span class="sxs-lookup"><span data-stu-id="ae341-136">Boolean</span></span>|<span data-ttu-id="ae341-137">如果附件显示为内嵌在嵌入对象的正文中，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="ae341-137">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="ae341-138">可选。</span><span class="sxs-lookup"><span data-stu-id="ae341-138">Optional.</span></span>|
|<span data-ttu-id="ae341-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae341-139">lastModifiedDateTime</span></span>|<span data-ttu-id="ae341-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae341-140">DateTimeOffset</span></span>|<span data-ttu-id="ae341-141">上次修改附件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="ae341-141">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="ae341-142">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="ae341-142">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ae341-143">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="ae341-143">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="ae341-144">可选。</span><span class="sxs-lookup"><span data-stu-id="ae341-144">Optional.</span></span>|
|<span data-ttu-id="ae341-145">name</span><span class="sxs-lookup"><span data-stu-id="ae341-145">name</span></span>|<span data-ttu-id="ae341-146">字符串</span><span class="sxs-lookup"><span data-stu-id="ae341-146">String</span></span>|<span data-ttu-id="ae341-147">表示嵌入的附件的图标下面显示的文本。</span><span class="sxs-lookup"><span data-stu-id="ae341-147">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="ae341-148">这不需要是实际的文件名称。</span><span class="sxs-lookup"><span data-stu-id="ae341-148">This does not need to be the actual file name.</span></span> <span data-ttu-id="ae341-149">必填。</span><span class="sxs-lookup"><span data-stu-id="ae341-149">Required.</span></span>|
|<span data-ttu-id="ae341-150">权限</span><span class="sxs-lookup"><span data-stu-id="ae341-150">permission</span></span>|<span data-ttu-id="ae341-151">ReferenceAttachmentPermissions</span><span class="sxs-lookup"><span data-stu-id="ae341-151">ReferenceAttachmentPermissions</span></span>|<span data-ttu-id="ae341-152">指定**提供程序类型**中的提供程序的类型为附件授予的权限。</span><span class="sxs-lookup"><span data-stu-id="ae341-152">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="ae341-153">可取值为：`other`、`view`、`edit`、`anonymousView`、`anonymousEdit`、`organizationView`、`organizationEdit`。</span><span class="sxs-lookup"><span data-stu-id="ae341-153">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="ae341-154">可选。</span><span class="sxs-lookup"><span data-stu-id="ae341-154">Optional.</span></span>|
|<span data-ttu-id="ae341-155">previewUrl</span><span class="sxs-lookup"><span data-stu-id="ae341-155">previewUrl</span></span>|<span data-ttu-id="ae341-156">字符串</span><span class="sxs-lookup"><span data-stu-id="ae341-156">String</span></span>|<span data-ttu-id="ae341-157">适用于仅图像-要获取的预览图像 URL 的参考附件。</span><span class="sxs-lookup"><span data-stu-id="ae341-157">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="ae341-158">仅当**sourceUrl**标识的图像文件，请使用**thumbnailUrl**和**previewUrl** 。</span><span class="sxs-lookup"><span data-stu-id="ae341-158">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="ae341-159">可选。</span><span class="sxs-lookup"><span data-stu-id="ae341-159">Optional.</span></span>|
|<span data-ttu-id="ae341-160">提供程序类型</span><span class="sxs-lookup"><span data-stu-id="ae341-160">providerType</span></span>|<span data-ttu-id="ae341-161">ReferenceAttachmentProviders</span><span class="sxs-lookup"><span data-stu-id="ae341-161">ReferenceAttachmentProviders</span></span>|<span data-ttu-id="ae341-162">支持此 contentType 的附件的提供程序的类型。</span><span class="sxs-lookup"><span data-stu-id="ae341-162">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="ae341-163">可取值为：`other`、`oneDriveBusiness`、`oneDriveConsumer`、`dropbox`。</span><span class="sxs-lookup"><span data-stu-id="ae341-163">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="ae341-164">可选。</span><span class="sxs-lookup"><span data-stu-id="ae341-164">Optional.</span></span>|
|<span data-ttu-id="ae341-165">size</span><span class="sxs-lookup"><span data-stu-id="ae341-165">size</span></span>|<span data-ttu-id="ae341-166">Int32</span><span class="sxs-lookup"><span data-stu-id="ae341-166">Int32</span></span>|<span data-ttu-id="ae341-167">存储在引用附件的邮件的元数据以字节为单位的大小。</span><span class="sxs-lookup"><span data-stu-id="ae341-167">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="ae341-168">此值不表示实际文件的大小。</span><span class="sxs-lookup"><span data-stu-id="ae341-168">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="ae341-169">可选。</span><span class="sxs-lookup"><span data-stu-id="ae341-169">Optional.</span></span>|
|<span data-ttu-id="ae341-170">sourceUrl</span><span class="sxs-lookup"><span data-stu-id="ae341-170">sourceUrl</span></span>|<span data-ttu-id="ae341-171">字符串</span><span class="sxs-lookup"><span data-stu-id="ae341-171">String</span></span>|<span data-ttu-id="ae341-172">若要获取附件内容的 URL。</span><span class="sxs-lookup"><span data-stu-id="ae341-172">URL to get the attachment content.</span></span> <span data-ttu-id="ae341-173">如果这是指向文件夹的 URL，然后为文件夹以在 Outlook 或 Outlook web 上的中正确显示设置**isFolder**为 true。</span><span class="sxs-lookup"><span data-stu-id="ae341-173">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="ae341-174">必填。</span><span class="sxs-lookup"><span data-stu-id="ae341-174">Required.</span></span>|
|<span data-ttu-id="ae341-175">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="ae341-175">thumbnailUrl</span></span>|<span data-ttu-id="ae341-176">字符串</span><span class="sxs-lookup"><span data-stu-id="ae341-176">String</span></span>|<span data-ttu-id="ae341-177">适用于仅图像-要获取的缩略图图像 URL 的参考附件。</span><span class="sxs-lookup"><span data-stu-id="ae341-177">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="ae341-178">仅当**sourceUrl**标识的图像文件，请使用**thumbnailUrl**和**previewUrl** 。</span><span class="sxs-lookup"><span data-stu-id="ae341-178">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="ae341-179">可选。</span><span class="sxs-lookup"><span data-stu-id="ae341-179">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae341-180">Relationships</span><span class="sxs-lookup"><span data-stu-id="ae341-180">Relationships</span></span>
<span data-ttu-id="ae341-181">无</span><span class="sxs-lookup"><span data-stu-id="ae341-181">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="ae341-182">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ae341-182">JSON representation</span></span>

<span data-ttu-id="ae341-183">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae341-183">Here is a JSON representation of the resource</span></span>

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
  "permission": "string",
  "previewUrl": "string",
  "providerType": "string",
  "size": 1024,
  "sourceUrl": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
