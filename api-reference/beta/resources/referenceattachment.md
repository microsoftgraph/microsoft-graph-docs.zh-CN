---
title: referenceAttachment 资源类型
description: '指向文件夹或文件的链接， (OneDrive for Business 云驱动器) 或其他受支持的存储位置上的文本文件或 Word 文档文件 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: 914d04a6482b96fda0ee55c92f25bf950e594173
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136764"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="5717b-103">referenceAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="5717b-103">referenceAttachment resource type</span></span>

<span data-ttu-id="5717b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5717b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5717b-105">指向附加到事件、 (或帖子的文件夹或文件（如 OneDrive for Business 云驱动器) 或其他受支持的存储位置上的文本文件或 Word 文档）[的链接](../resources/post.md)。 [](../resources/event.md) [](../resources/message.md)</span><span class="sxs-lookup"><span data-stu-id="5717b-105">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="5717b-106">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="5717b-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="5717b-107">方法</span><span class="sxs-lookup"><span data-stu-id="5717b-107">Methods</span></span>

| <span data-ttu-id="5717b-108">方法</span><span class="sxs-lookup"><span data-stu-id="5717b-108">Method</span></span>       | <span data-ttu-id="5717b-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="5717b-109">Return Type</span></span>  |<span data-ttu-id="5717b-110">说明</span><span class="sxs-lookup"><span data-stu-id="5717b-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5717b-111">获取</span><span class="sxs-lookup"><span data-stu-id="5717b-111">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="5717b-112">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="5717b-112">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="5717b-113">读取 referenceAttachment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5717b-113">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="5717b-114">删除</span><span class="sxs-lookup"><span data-stu-id="5717b-114">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="5717b-115">无</span><span class="sxs-lookup"><span data-stu-id="5717b-115">None</span></span> |<span data-ttu-id="5717b-116">删除 referenceAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="5717b-116">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="5717b-117">属性</span><span class="sxs-lookup"><span data-stu-id="5717b-117">Properties</span></span>
| <span data-ttu-id="5717b-118">属性</span><span class="sxs-lookup"><span data-stu-id="5717b-118">Property</span></span>     | <span data-ttu-id="5717b-119">类型</span><span class="sxs-lookup"><span data-stu-id="5717b-119">Type</span></span>   |<span data-ttu-id="5717b-120">说明</span><span class="sxs-lookup"><span data-stu-id="5717b-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5717b-121">contentType</span><span class="sxs-lookup"><span data-stu-id="5717b-121">contentType</span></span>|<span data-ttu-id="5717b-122">String</span><span class="sxs-lookup"><span data-stu-id="5717b-122">String</span></span>|<span data-ttu-id="5717b-123">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="5717b-123">The content type of the attachment.</span></span> <span data-ttu-id="5717b-124">可选。</span><span class="sxs-lookup"><span data-stu-id="5717b-124">Optional.</span></span>|
|<span data-ttu-id="5717b-125">id</span><span class="sxs-lookup"><span data-stu-id="5717b-125">id</span></span>|<span data-ttu-id="5717b-126">字符串</span><span class="sxs-lookup"><span data-stu-id="5717b-126">String</span></span>|<span data-ttu-id="5717b-p102">附件 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="5717b-p102">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="5717b-129">isFolder</span><span class="sxs-lookup"><span data-stu-id="5717b-129">isFolder</span></span>|<span data-ttu-id="5717b-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="5717b-130">Boolean</span></span>|<span data-ttu-id="5717b-131">指定附件是否是指向文件夹的链接。</span><span class="sxs-lookup"><span data-stu-id="5717b-131">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="5717b-132">如果 **sourceUrl** 是指向文件夹的链接，则必须将此选项设置为 true。</span><span class="sxs-lookup"><span data-stu-id="5717b-132">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="5717b-133">可选。</span><span class="sxs-lookup"><span data-stu-id="5717b-133">Optional.</span></span>|
|<span data-ttu-id="5717b-134">isInline</span><span class="sxs-lookup"><span data-stu-id="5717b-134">isInline</span></span>|<span data-ttu-id="5717b-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="5717b-135">Boolean</span></span>|<span data-ttu-id="5717b-136">如果附件显示为内嵌在嵌入对象的正文中，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="5717b-136">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="5717b-137">可选。</span><span class="sxs-lookup"><span data-stu-id="5717b-137">Optional.</span></span>|
|<span data-ttu-id="5717b-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5717b-138">lastModifiedDateTime</span></span>|<span data-ttu-id="5717b-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5717b-139">DateTimeOffset</span></span>|<span data-ttu-id="5717b-140">上次修改附件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="5717b-140">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="5717b-141">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="5717b-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5717b-142">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="5717b-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="5717b-143">可选。</span><span class="sxs-lookup"><span data-stu-id="5717b-143">Optional.</span></span>|
|<span data-ttu-id="5717b-144">name</span><span class="sxs-lookup"><span data-stu-id="5717b-144">name</span></span>|<span data-ttu-id="5717b-145">字符串</span><span class="sxs-lookup"><span data-stu-id="5717b-145">String</span></span>|<span data-ttu-id="5717b-146">显示在用于表示嵌入附件的图标下方的文本。</span><span class="sxs-lookup"><span data-stu-id="5717b-146">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="5717b-147">这不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="5717b-147">This does not need to be the actual file name.</span></span> <span data-ttu-id="5717b-148">必填。</span><span class="sxs-lookup"><span data-stu-id="5717b-148">Required.</span></span>|
|<span data-ttu-id="5717b-149">permission</span><span class="sxs-lookup"><span data-stu-id="5717b-149">permission</span></span>|<span data-ttu-id="5717b-150">referenceAttachmentPermission</span><span class="sxs-lookup"><span data-stu-id="5717b-150">referenceAttachmentPermission</span></span>|<span data-ttu-id="5717b-151">指定通过 providerType 中的提供程序类型为附件 **授予的权限**。</span><span class="sxs-lookup"><span data-stu-id="5717b-151">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="5717b-152">可取值为：`other`、`view`、`edit`、`anonymousView`、`anonymousEdit`、`organizationView` 或 `organizationEdit`。</span><span class="sxs-lookup"><span data-stu-id="5717b-152">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="5717b-153">可选。</span><span class="sxs-lookup"><span data-stu-id="5717b-153">Optional.</span></span>|
|<span data-ttu-id="5717b-154">previewUrl</span><span class="sxs-lookup"><span data-stu-id="5717b-154">previewUrl</span></span>|<span data-ttu-id="5717b-155">字符串</span><span class="sxs-lookup"><span data-stu-id="5717b-155">String</span></span>|<span data-ttu-id="5717b-156">仅适用于图像的引用附件 - 用于获取预览图像的 URL。</span><span class="sxs-lookup"><span data-stu-id="5717b-156">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="5717b-157">仅在 sourceUrl 标识图像文件时，才使用 **thumbnailUrl** 和 **previewUrl。** </span><span class="sxs-lookup"><span data-stu-id="5717b-157">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="5717b-158">可选。</span><span class="sxs-lookup"><span data-stu-id="5717b-158">Optional.</span></span>|
|<span data-ttu-id="5717b-159">providerType</span><span class="sxs-lookup"><span data-stu-id="5717b-159">providerType</span></span>|<span data-ttu-id="5717b-160">referenceAttachmentProvider</span><span class="sxs-lookup"><span data-stu-id="5717b-160">referenceAttachmentProvider</span></span>|<span data-ttu-id="5717b-161">支持此 contentType 的附件的提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="5717b-161">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="5717b-162">可取值为：`other`、`oneDriveBusiness`、`oneDriveConsumer`、`dropbox`。</span><span class="sxs-lookup"><span data-stu-id="5717b-162">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="5717b-163">可选。</span><span class="sxs-lookup"><span data-stu-id="5717b-163">Optional.</span></span>|
|<span data-ttu-id="5717b-164">大小</span><span class="sxs-lookup"><span data-stu-id="5717b-164">size</span></span>|<span data-ttu-id="5717b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5717b-165">Int32</span></span>|<span data-ttu-id="5717b-166">用于引用附件的邮件中存储的元数据的大小（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="5717b-166">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="5717b-167">此值不表示实际文件的大小。</span><span class="sxs-lookup"><span data-stu-id="5717b-167">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="5717b-168">可选。</span><span class="sxs-lookup"><span data-stu-id="5717b-168">Optional.</span></span>|
|<span data-ttu-id="5717b-169">sourceUrl</span><span class="sxs-lookup"><span data-stu-id="5717b-169">sourceUrl</span></span>|<span data-ttu-id="5717b-170">字符串</span><span class="sxs-lookup"><span data-stu-id="5717b-170">String</span></span>|<span data-ttu-id="5717b-171">用于获取附件内容的 URL。</span><span class="sxs-lookup"><span data-stu-id="5717b-171">URL to get the attachment content.</span></span> <span data-ttu-id="5717b-172">如果这是文件夹的 URL，则对于要正确显示在 Outlook 或 Web 上的 Outlook 中的文件夹，将 **isFolder** 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="5717b-172">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="5717b-173">必填。</span><span class="sxs-lookup"><span data-stu-id="5717b-173">Required.</span></span>|
|<span data-ttu-id="5717b-174">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="5717b-174">thumbnailUrl</span></span>|<span data-ttu-id="5717b-175">字符串</span><span class="sxs-lookup"><span data-stu-id="5717b-175">String</span></span>|<span data-ttu-id="5717b-176">仅适用于图像的引用附件 - 用于获取缩略图的 URL。</span><span class="sxs-lookup"><span data-stu-id="5717b-176">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="5717b-177">仅在 sourceUrl 标识图像文件时，才使用 **thumbnailUrl** 和 **previewUrl。** </span><span class="sxs-lookup"><span data-stu-id="5717b-177">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="5717b-178">可选。</span><span class="sxs-lookup"><span data-stu-id="5717b-178">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5717b-179">关系</span><span class="sxs-lookup"><span data-stu-id="5717b-179">Relationships</span></span>
<span data-ttu-id="5717b-180">无</span><span class="sxs-lookup"><span data-stu-id="5717b-180">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="5717b-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5717b-181">JSON representation</span></span>

<span data-ttu-id="5717b-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5717b-182">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.attachment",
  "keyProperty":"id",
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


