---
title: hasPayloadLinkResultItem 资源类型
description: 包含 HasPayloadLinks 操作结果的类。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 46568e386c2896db307f78cc12205c115605a76e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42775904"
---
# <a name="haspayloadlinkresultitem-resource-type"></a><span data-ttu-id="b8586-103">hasPayloadLinkResultItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="b8586-103">hasPayloadLinkResultItem resource type</span></span>

> <span data-ttu-id="b8586-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b8586-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8586-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b8586-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8586-106">包含 HasPayloadLinks 操作结果的类。</span><span class="sxs-lookup"><span data-stu-id="b8586-106">A class containing the result of HasPayloadLinks action.</span></span>

## <a name="properties"></a><span data-ttu-id="b8586-107">属性</span><span class="sxs-lookup"><span data-stu-id="b8586-107">Properties</span></span>
|<span data-ttu-id="b8586-108">属性</span><span class="sxs-lookup"><span data-stu-id="b8586-108">Property</span></span>|<span data-ttu-id="b8586-109">类型</span><span class="sxs-lookup"><span data-stu-id="b8586-109">Type</span></span>|<span data-ttu-id="b8586-110">说明</span><span class="sxs-lookup"><span data-stu-id="b8586-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8586-111">payloadId</span><span class="sxs-lookup"><span data-stu-id="b8586-111">payloadId</span></span>|<span data-ttu-id="b8586-112">String</span><span class="sxs-lookup"><span data-stu-id="b8586-112">String</span></span>|<span data-ttu-id="b8586-113">有效负载的键，格式为 Guid。</span><span class="sxs-lookup"><span data-stu-id="b8586-113">Key of the Payload, In the format of Guid.</span></span>|
|<span data-ttu-id="b8586-114">hasLink</span><span class="sxs-lookup"><span data-stu-id="b8586-114">hasLink</span></span>|<span data-ttu-id="b8586-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="b8586-115">Boolean</span></span>|<span data-ttu-id="b8586-116">指示有效负载是否有任何链接。</span><span class="sxs-lookup"><span data-stu-id="b8586-116">Indicate whether a payload has any link or not.</span></span>|
|<span data-ttu-id="b8586-117">error</span><span class="sxs-lookup"><span data-stu-id="b8586-117">error</span></span>|<span data-ttu-id="b8586-118">String</span><span class="sxs-lookup"><span data-stu-id="b8586-118">String</span></span>|<span data-ttu-id="b8586-119">异常信息指示是否成功检查此项。空字符串表示无错误。</span><span class="sxs-lookup"><span data-stu-id="b8586-119">Exception information indicates if check for this item was successful or not.Empty string for no error.</span></span>|
|<span data-ttu-id="b8586-120">源</span><span class="sxs-lookup"><span data-stu-id="b8586-120">sources</span></span>|<span data-ttu-id="b8586-121">[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md)集合</span><span class="sxs-lookup"><span data-stu-id="b8586-121">[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md) collection</span></span>|<span data-ttu-id="b8586-122">链接来自的原因。</span><span class="sxs-lookup"><span data-stu-id="b8586-122">The reason where the link comes from.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8586-123">关系</span><span class="sxs-lookup"><span data-stu-id="b8586-123">Relationships</span></span>
<span data-ttu-id="b8586-124">无</span><span class="sxs-lookup"><span data-stu-id="b8586-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8586-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b8586-125">JSON Representation</span></span>
<span data-ttu-id="b8586-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8586-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hasPayloadLinkResultItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hasPayloadLinkResultItem",
  "payloadId": "String",
  "hasLink": true,
  "error": "String",
  "sources": [
    "String"
  ]
}
```



