---
title: referenceAttachment 资源类型
description: 'OneDrive for Business 云驱动器上的文件夹或文件 (如文本文件或 Word 文档) 的链接, 或附加到的其他受支持的存储位置 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: ef3e2dd5292ee018c0b72c29c8bd6c33fed00f11
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008710"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="d08f2-103">referenceAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="d08f2-103">referenceAttachment resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d08f2-104">OneDrive for Business 云驱动器上的文件夹或文件 (如文本文件或 Word 文档) 的链接, 以及附加到[事件](../resources/event.md)、[邮件](../resources/message.md)、 [Outlook 任务](../resources/outlooktask.md)或[公告](../resources/post.md)的其他受支持的存储位置。</span><span class="sxs-lookup"><span data-stu-id="d08f2-104">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), [Outlook task](../resources/outlooktask.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="d08f2-105">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="d08f2-105">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="d08f2-106">方法</span><span class="sxs-lookup"><span data-stu-id="d08f2-106">Methods</span></span>

| <span data-ttu-id="d08f2-107">方法</span><span class="sxs-lookup"><span data-stu-id="d08f2-107">Method</span></span>       | <span data-ttu-id="d08f2-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d08f2-108">Return Type</span></span>  |<span data-ttu-id="d08f2-109">说明</span><span class="sxs-lookup"><span data-stu-id="d08f2-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d08f2-110">Get</span><span class="sxs-lookup"><span data-stu-id="d08f2-110">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="d08f2-111">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="d08f2-111">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="d08f2-112">读取 referenceAttachment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d08f2-112">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="d08f2-113">删除</span><span class="sxs-lookup"><span data-stu-id="d08f2-113">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="d08f2-114">无</span><span class="sxs-lookup"><span data-stu-id="d08f2-114">None</span></span> |<span data-ttu-id="d08f2-115">删除 referenceAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="d08f2-115">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d08f2-116">属性</span><span class="sxs-lookup"><span data-stu-id="d08f2-116">Properties</span></span>
| <span data-ttu-id="d08f2-117">属性</span><span class="sxs-lookup"><span data-stu-id="d08f2-117">Property</span></span>     | <span data-ttu-id="d08f2-118">类型</span><span class="sxs-lookup"><span data-stu-id="d08f2-118">Type</span></span>   |<span data-ttu-id="d08f2-119">说明</span><span class="sxs-lookup"><span data-stu-id="d08f2-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d08f2-120">contentType</span><span class="sxs-lookup"><span data-stu-id="d08f2-120">contentType</span></span>|<span data-ttu-id="d08f2-121">String</span><span class="sxs-lookup"><span data-stu-id="d08f2-121">String</span></span>|<span data-ttu-id="d08f2-122">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="d08f2-122">The content type of the attachment.</span></span> <span data-ttu-id="d08f2-123">可选。</span><span class="sxs-lookup"><span data-stu-id="d08f2-123">Optional.</span></span>|
|<span data-ttu-id="d08f2-124">id</span><span class="sxs-lookup"><span data-stu-id="d08f2-124">id</span></span>|<span data-ttu-id="d08f2-125">String</span><span class="sxs-lookup"><span data-stu-id="d08f2-125">String</span></span>|<span data-ttu-id="d08f2-p102">附件 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="d08f2-p102">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="d08f2-128">isFolder</span><span class="sxs-lookup"><span data-stu-id="d08f2-128">isFolder</span></span>|<span data-ttu-id="d08f2-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="d08f2-129">Boolean</span></span>|<span data-ttu-id="d08f2-130">指定附件是否为文件夹的链接。</span><span class="sxs-lookup"><span data-stu-id="d08f2-130">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="d08f2-131">如果**sourceUrl**是指向文件夹的链接, 则必须将其设置为 true。</span><span class="sxs-lookup"><span data-stu-id="d08f2-131">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="d08f2-132">可选。</span><span class="sxs-lookup"><span data-stu-id="d08f2-132">Optional.</span></span>|
|<span data-ttu-id="d08f2-133">isInline</span><span class="sxs-lookup"><span data-stu-id="d08f2-133">isInline</span></span>|<span data-ttu-id="d08f2-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="d08f2-134">Boolean</span></span>|<span data-ttu-id="d08f2-135">如果附件显示为内嵌在嵌入对象的正文中，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="d08f2-135">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="d08f2-136">可选。</span><span class="sxs-lookup"><span data-stu-id="d08f2-136">Optional.</span></span>|
|<span data-ttu-id="d08f2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d08f2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d08f2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d08f2-138">DateTimeOffset</span></span>|<span data-ttu-id="d08f2-139">上次修改附件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d08f2-139">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="d08f2-140">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="d08f2-140">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d08f2-141">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="d08f2-141">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="d08f2-142">可选。</span><span class="sxs-lookup"><span data-stu-id="d08f2-142">Optional.</span></span>|
|<span data-ttu-id="d08f2-143">name</span><span class="sxs-lookup"><span data-stu-id="d08f2-143">name</span></span>|<span data-ttu-id="d08f2-144">字符串</span><span class="sxs-lookup"><span data-stu-id="d08f2-144">String</span></span>|<span data-ttu-id="d08f2-145">显示在用于表示嵌入附件的图标下方的文本。</span><span class="sxs-lookup"><span data-stu-id="d08f2-145">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="d08f2-146">这不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="d08f2-146">This does not need to be the actual file name.</span></span> <span data-ttu-id="d08f2-147">必需。</span><span class="sxs-lookup"><span data-stu-id="d08f2-147">Required.</span></span>|
|<span data-ttu-id="d08f2-148">拒绝</span><span class="sxs-lookup"><span data-stu-id="d08f2-148">permission</span></span>|<span data-ttu-id="d08f2-149">referenceAttachmentPermission</span><span class="sxs-lookup"><span data-stu-id="d08f2-149">referenceAttachmentPermission</span></span>|<span data-ttu-id="d08f2-150">指定通过**providerType**中的提供程序类型授予附件的权限。</span><span class="sxs-lookup"><span data-stu-id="d08f2-150">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="d08f2-151">可取值为：`other`、`view`、`edit`、`anonymousView`、`anonymousEdit`、`organizationView` 或 `organizationEdit`。</span><span class="sxs-lookup"><span data-stu-id="d08f2-151">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="d08f2-152">可选。</span><span class="sxs-lookup"><span data-stu-id="d08f2-152">Optional.</span></span>|
|<span data-ttu-id="d08f2-153">previewUrl</span><span class="sxs-lookup"><span data-stu-id="d08f2-153">previewUrl</span></span>|<span data-ttu-id="d08f2-154">String</span><span class="sxs-lookup"><span data-stu-id="d08f2-154">String</span></span>|<span data-ttu-id="d08f2-155">仅适用于图像 URL 的引用附件, 以获取预览图像。</span><span class="sxs-lookup"><span data-stu-id="d08f2-155">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="d08f2-156">仅当**sourceUrl**标识图像文件时, 才使用**thumbnailUrl**和**previewUrl** 。</span><span class="sxs-lookup"><span data-stu-id="d08f2-156">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="d08f2-157">可选。</span><span class="sxs-lookup"><span data-stu-id="d08f2-157">Optional.</span></span>|
|<span data-ttu-id="d08f2-158">providerType</span><span class="sxs-lookup"><span data-stu-id="d08f2-158">providerType</span></span>|<span data-ttu-id="d08f2-159">: Referenceattachmentprovider</span><span class="sxs-lookup"><span data-stu-id="d08f2-159">referenceAttachmentProvider</span></span>|<span data-ttu-id="d08f2-160">支持此 contentType 的附件的提供程序的类型。</span><span class="sxs-lookup"><span data-stu-id="d08f2-160">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="d08f2-161">可取值为：`other`、`oneDriveBusiness`、`oneDriveConsumer`、`dropbox`。</span><span class="sxs-lookup"><span data-stu-id="d08f2-161">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="d08f2-162">可选。</span><span class="sxs-lookup"><span data-stu-id="d08f2-162">Optional.</span></span>|
|<span data-ttu-id="d08f2-163">size</span><span class="sxs-lookup"><span data-stu-id="d08f2-163">size</span></span>|<span data-ttu-id="d08f2-164">Int32</span><span class="sxs-lookup"><span data-stu-id="d08f2-164">Int32</span></span>|<span data-ttu-id="d08f2-165">存储在引用附件的邮件上的元数据的大小 (以字节为单位)。</span><span class="sxs-lookup"><span data-stu-id="d08f2-165">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="d08f2-166">此值不表示实际文件的大小。</span><span class="sxs-lookup"><span data-stu-id="d08f2-166">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="d08f2-167">可选。</span><span class="sxs-lookup"><span data-stu-id="d08f2-167">Optional.</span></span>|
|<span data-ttu-id="d08f2-168">sourceUrl</span><span class="sxs-lookup"><span data-stu-id="d08f2-168">sourceUrl</span></span>|<span data-ttu-id="d08f2-169">String</span><span class="sxs-lookup"><span data-stu-id="d08f2-169">String</span></span>|<span data-ttu-id="d08f2-170">用于获取附件内容的 URL。</span><span class="sxs-lookup"><span data-stu-id="d08f2-170">URL to get the attachment content.</span></span> <span data-ttu-id="d08f2-171">如果这是指向文件夹的 URL, 然后在 Outlook 或 web 上的 Outlook 中正确显示该文件夹, 请将**isFolder**设置为 true。</span><span class="sxs-lookup"><span data-stu-id="d08f2-171">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="d08f2-172">必需。</span><span class="sxs-lookup"><span data-stu-id="d08f2-172">Required.</span></span>|
|<span data-ttu-id="d08f2-173">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="d08f2-173">thumbnailUrl</span></span>|<span data-ttu-id="d08f2-174">String</span><span class="sxs-lookup"><span data-stu-id="d08f2-174">String</span></span>|<span data-ttu-id="d08f2-175">仅适用于图像 URL 的引用附件, 以获取缩略图图像。</span><span class="sxs-lookup"><span data-stu-id="d08f2-175">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="d08f2-176">仅当**sourceUrl**标识图像文件时, 才使用**thumbnailUrl**和**previewUrl** 。</span><span class="sxs-lookup"><span data-stu-id="d08f2-176">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="d08f2-177">可选。</span><span class="sxs-lookup"><span data-stu-id="d08f2-177">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d08f2-178">关系</span><span class="sxs-lookup"><span data-stu-id="d08f2-178">Relationships</span></span>
<span data-ttu-id="d08f2-179">无</span><span class="sxs-lookup"><span data-stu-id="d08f2-179">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="d08f2-180">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d08f2-180">JSON representation</span></span>

<span data-ttu-id="d08f2-181">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d08f2-181">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "referenceAttachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
