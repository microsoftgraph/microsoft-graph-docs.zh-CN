---
title: referenceAttachment 资源类型
description: 'OneDrive for Business 云驱动器上的文件夹或文件（如文本文件或 Word 文档）的链接，或附加到的其他受支持的存储位置 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: angelgolfer-ms
ms.openlocfilehash: c338e80d7a816bb583a4f6b3923f7e23990a64a5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521199"
---
# <a name="referenceattachment-resource-type"></a><span data-ttu-id="c912e-103">referenceAttachment 资源类型</span><span class="sxs-lookup"><span data-stu-id="c912e-103">referenceAttachment resource type</span></span>

<span data-ttu-id="c912e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c912e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c912e-105">OneDrive for Business 云驱动器上的文件夹或文件（如文本文件或 Word 文档）的链接，或附加到[事件](../resources/event.md)、[邮件](../resources/message.md)或[公告](../resources/post.md)的其他受支持的存储位置。</span><span class="sxs-lookup"><span data-stu-id="c912e-105">A link to a folder or file (such as a text file or Word document) on a OneDrive for Business cloud drive, or other supported storage locations, attached to an [event](../resources/event.md), [message](../resources/message.md), or [post](../resources/post.md) .</span></span>

<span data-ttu-id="c912e-106">派生自 [附件](attachment.md)。</span><span class="sxs-lookup"><span data-stu-id="c912e-106">Derived from [attachment](attachment.md).</span></span>

## <a name="methods"></a><span data-ttu-id="c912e-107">方法</span><span class="sxs-lookup"><span data-stu-id="c912e-107">Methods</span></span>

| <span data-ttu-id="c912e-108">方法</span><span class="sxs-lookup"><span data-stu-id="c912e-108">Method</span></span>       | <span data-ttu-id="c912e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="c912e-109">Return Type</span></span>  |<span data-ttu-id="c912e-110">说明</span><span class="sxs-lookup"><span data-stu-id="c912e-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c912e-111">获取</span><span class="sxs-lookup"><span data-stu-id="c912e-111">Get</span></span>](../api/attachment-get.md) | [<span data-ttu-id="c912e-112">referenceAttachment</span><span class="sxs-lookup"><span data-stu-id="c912e-112">referenceAttachment</span></span>](referenceattachment.md) |<span data-ttu-id="c912e-113">读取 referenceAttachment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c912e-113">Read properties and relationships of referenceAttachment object.</span></span>|
|[<span data-ttu-id="c912e-114">删除</span><span class="sxs-lookup"><span data-stu-id="c912e-114">Delete</span></span>](../api/attachment-delete.md) | <span data-ttu-id="c912e-115">无</span><span class="sxs-lookup"><span data-stu-id="c912e-115">None</span></span> |<span data-ttu-id="c912e-116">删除 referenceAttachment 对象。</span><span class="sxs-lookup"><span data-stu-id="c912e-116">Delete referenceAttachment object.</span></span> |

## <a name="properties"></a><span data-ttu-id="c912e-117">属性</span><span class="sxs-lookup"><span data-stu-id="c912e-117">Properties</span></span>
| <span data-ttu-id="c912e-118">属性</span><span class="sxs-lookup"><span data-stu-id="c912e-118">Property</span></span>     | <span data-ttu-id="c912e-119">类型</span><span class="sxs-lookup"><span data-stu-id="c912e-119">Type</span></span>   |<span data-ttu-id="c912e-120">说明</span><span class="sxs-lookup"><span data-stu-id="c912e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c912e-121">contentType</span><span class="sxs-lookup"><span data-stu-id="c912e-121">contentType</span></span>|<span data-ttu-id="c912e-122">String</span><span class="sxs-lookup"><span data-stu-id="c912e-122">String</span></span>|<span data-ttu-id="c912e-123">附件的内容类型。</span><span class="sxs-lookup"><span data-stu-id="c912e-123">The content type of the attachment.</span></span> <span data-ttu-id="c912e-124">可选。</span><span class="sxs-lookup"><span data-stu-id="c912e-124">Optional.</span></span>|
|<span data-ttu-id="c912e-125">id</span><span class="sxs-lookup"><span data-stu-id="c912e-125">id</span></span>|<span data-ttu-id="c912e-126">String</span><span class="sxs-lookup"><span data-stu-id="c912e-126">String</span></span>|<span data-ttu-id="c912e-p102">附件 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="c912e-p102">The attachment ID.  Read-only.</span></span>|
|<span data-ttu-id="c912e-129">isFolder</span><span class="sxs-lookup"><span data-stu-id="c912e-129">isFolder</span></span>|<span data-ttu-id="c912e-130">布尔</span><span class="sxs-lookup"><span data-stu-id="c912e-130">Boolean</span></span>|<span data-ttu-id="c912e-131">指定附件是否为文件夹的链接。</span><span class="sxs-lookup"><span data-stu-id="c912e-131">Specifies whether the attachment is a link to a folder.</span></span> <span data-ttu-id="c912e-132">如果**sourceUrl**是指向文件夹的链接，则必须将其设置为 true。</span><span class="sxs-lookup"><span data-stu-id="c912e-132">Must set this to true if **sourceUrl** is a link to a folder.</span></span> <span data-ttu-id="c912e-133">可选。</span><span class="sxs-lookup"><span data-stu-id="c912e-133">Optional.</span></span>|
|<span data-ttu-id="c912e-134">isInline</span><span class="sxs-lookup"><span data-stu-id="c912e-134">isInline</span></span>|<span data-ttu-id="c912e-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="c912e-135">Boolean</span></span>|<span data-ttu-id="c912e-136">如果附件显示为内嵌在嵌入对象的正文中，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="c912e-136">Set to true if the attachment appears inline in the body of the embedding object.</span></span> <span data-ttu-id="c912e-137">可选。</span><span class="sxs-lookup"><span data-stu-id="c912e-137">Optional.</span></span>|
|<span data-ttu-id="c912e-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c912e-138">lastModifiedDateTime</span></span>|<span data-ttu-id="c912e-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c912e-139">DateTimeOffset</span></span>|<span data-ttu-id="c912e-140">上次修改附件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="c912e-140">The date and time when the attachment was last modified.</span></span> <span data-ttu-id="c912e-141">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="c912e-141">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c912e-142">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="c912e-142">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="c912e-143">可选。</span><span class="sxs-lookup"><span data-stu-id="c912e-143">Optional.</span></span>|
|<span data-ttu-id="c912e-144">name</span><span class="sxs-lookup"><span data-stu-id="c912e-144">name</span></span>|<span data-ttu-id="c912e-145">字符串</span><span class="sxs-lookup"><span data-stu-id="c912e-145">String</span></span>|<span data-ttu-id="c912e-146">显示在用于表示嵌入附件的图标下方的文本。</span><span class="sxs-lookup"><span data-stu-id="c912e-146">The text that is displayed below the icon representing the embedded attachment.</span></span> <span data-ttu-id="c912e-147">这不必是实际的文件名。</span><span class="sxs-lookup"><span data-stu-id="c912e-147">This does not need to be the actual file name.</span></span> <span data-ttu-id="c912e-148">必填。</span><span class="sxs-lookup"><span data-stu-id="c912e-148">Required.</span></span>|
|<span data-ttu-id="c912e-149">拒绝</span><span class="sxs-lookup"><span data-stu-id="c912e-149">permission</span></span>|<span data-ttu-id="c912e-150">referenceAttachmentPermission</span><span class="sxs-lookup"><span data-stu-id="c912e-150">referenceAttachmentPermission</span></span>|<span data-ttu-id="c912e-151">指定通过**providerType**中的提供程序类型授予附件的权限。</span><span class="sxs-lookup"><span data-stu-id="c912e-151">Specifies the permissions granted for the attachment by the type of provider in **providerType**.</span></span> <span data-ttu-id="c912e-152">可取值为：`other`、`view`、`edit`、`anonymousView`、`anonymousEdit`、`organizationView` 或 `organizationEdit`。</span><span class="sxs-lookup"><span data-stu-id="c912e-152">Possible values are: `other`, `view`, `edit`, `anonymousView`, `anonymousEdit`, `organizationView`, `organizationEdit`.</span></span> <span data-ttu-id="c912e-153">可选。</span><span class="sxs-lookup"><span data-stu-id="c912e-153">Optional.</span></span>|
|<span data-ttu-id="c912e-154">previewUrl</span><span class="sxs-lookup"><span data-stu-id="c912e-154">previewUrl</span></span>|<span data-ttu-id="c912e-155">String</span><span class="sxs-lookup"><span data-stu-id="c912e-155">String</span></span>|<span data-ttu-id="c912e-156">仅适用于图像 URL 的引用附件，以获取预览图像。</span><span class="sxs-lookup"><span data-stu-id="c912e-156">Applies to only a reference attachment of an image - URL to get a preview image.</span></span> <span data-ttu-id="c912e-157">仅当**sourceUrl**标识图像文件时，才使用**thumbnailUrl**和**previewUrl** 。</span><span class="sxs-lookup"><span data-stu-id="c912e-157">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="c912e-158">可选。</span><span class="sxs-lookup"><span data-stu-id="c912e-158">Optional.</span></span>|
|<span data-ttu-id="c912e-159">providerType</span><span class="sxs-lookup"><span data-stu-id="c912e-159">providerType</span></span>|<span data-ttu-id="c912e-160">： Referenceattachmentprovider</span><span class="sxs-lookup"><span data-stu-id="c912e-160">referenceAttachmentProvider</span></span>|<span data-ttu-id="c912e-161">支持此 contentType 的附件的提供程序的类型。</span><span class="sxs-lookup"><span data-stu-id="c912e-161">The type of provider that supports an attachment of this contentType.</span></span> <span data-ttu-id="c912e-162">可取值为：`other`、`oneDriveBusiness`、`oneDriveConsumer`、`dropbox`。</span><span class="sxs-lookup"><span data-stu-id="c912e-162">Possible values are: `other`, `oneDriveBusiness`, `oneDriveConsumer`, `dropbox`.</span></span> <span data-ttu-id="c912e-163">可选。</span><span class="sxs-lookup"><span data-stu-id="c912e-163">Optional.</span></span>|
|<span data-ttu-id="c912e-164">size</span><span class="sxs-lookup"><span data-stu-id="c912e-164">size</span></span>|<span data-ttu-id="c912e-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c912e-165">Int32</span></span>|<span data-ttu-id="c912e-166">存储在引用附件的邮件上的元数据的大小（以字节为单位）。</span><span class="sxs-lookup"><span data-stu-id="c912e-166">The size of the metadata in bytes that is stored on the message for the reference attachment.</span></span> <span data-ttu-id="c912e-167">此值不表示实际文件的大小。</span><span class="sxs-lookup"><span data-stu-id="c912e-167">This value does not indicate the size of the actual file.</span></span> <span data-ttu-id="c912e-168">可选。</span><span class="sxs-lookup"><span data-stu-id="c912e-168">Optional.</span></span>|
|<span data-ttu-id="c912e-169">sourceUrl</span><span class="sxs-lookup"><span data-stu-id="c912e-169">sourceUrl</span></span>|<span data-ttu-id="c912e-170">String</span><span class="sxs-lookup"><span data-stu-id="c912e-170">String</span></span>|<span data-ttu-id="c912e-171">用于获取附件内容的 URL。</span><span class="sxs-lookup"><span data-stu-id="c912e-171">URL to get the attachment content.</span></span> <span data-ttu-id="c912e-172">如果这是指向文件夹的 URL，然后在 Outlook 或 web 上的 Outlook 中正确显示该文件夹，请将**isFolder**设置为 true。</span><span class="sxs-lookup"><span data-stu-id="c912e-172">If this is a URL to a folder, then for the folder to be displayed correctly in Outlook or Outlook on the web, set **isFolder** to true.</span></span> <span data-ttu-id="c912e-173">必填。</span><span class="sxs-lookup"><span data-stu-id="c912e-173">Required.</span></span>|
|<span data-ttu-id="c912e-174">thumbnailUrl</span><span class="sxs-lookup"><span data-stu-id="c912e-174">thumbnailUrl</span></span>|<span data-ttu-id="c912e-175">String</span><span class="sxs-lookup"><span data-stu-id="c912e-175">String</span></span>|<span data-ttu-id="c912e-176">仅适用于图像 URL 的引用附件，以获取缩略图图像。</span><span class="sxs-lookup"><span data-stu-id="c912e-176">Applies to only a reference attachment of an image - URL to get a thumbnail image.</span></span> <span data-ttu-id="c912e-177">仅当**sourceUrl**标识图像文件时，才使用**thumbnailUrl**和**previewUrl** 。</span><span class="sxs-lookup"><span data-stu-id="c912e-177">Use **thumbnailUrl** and **previewUrl** only when **sourceUrl** identifies an image file.</span></span> <span data-ttu-id="c912e-178">可选。</span><span class="sxs-lookup"><span data-stu-id="c912e-178">Optional.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c912e-179">关系</span><span class="sxs-lookup"><span data-stu-id="c912e-179">Relationships</span></span>
<span data-ttu-id="c912e-180">无</span><span class="sxs-lookup"><span data-stu-id="c912e-180">None</span></span>



## <a name="json-representation"></a><span data-ttu-id="c912e-181">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c912e-181">JSON representation</span></span>

<span data-ttu-id="c912e-182">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c912e-182">Here is a JSON representation of the resource</span></span>

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
