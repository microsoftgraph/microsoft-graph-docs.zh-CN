---
title: hasPayloadLinkResultItem 资源类型
description: 包含 HasPayloadLinks 操作结果的类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 09e61f33151158c600e3a3ea783965f2f131fcce
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199972"
---
# <a name="haspayloadlinkresultitem-resource-type"></a><span data-ttu-id="0be55-103">hasPayloadLinkResultItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="0be55-103">hasPayloadLinkResultItem resource type</span></span>

> <span data-ttu-id="0be55-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0be55-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0be55-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0be55-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0be55-106">包含 HasPayloadLinks 操作结果的类。</span><span class="sxs-lookup"><span data-stu-id="0be55-106">A class containing the result of HasPayloadLinks action.</span></span>

## <a name="properties"></a><span data-ttu-id="0be55-107">属性</span><span class="sxs-lookup"><span data-stu-id="0be55-107">Properties</span></span>
|<span data-ttu-id="0be55-108">属性</span><span class="sxs-lookup"><span data-stu-id="0be55-108">Property</span></span>|<span data-ttu-id="0be55-109">类型</span><span class="sxs-lookup"><span data-stu-id="0be55-109">Type</span></span>|<span data-ttu-id="0be55-110">说明</span><span class="sxs-lookup"><span data-stu-id="0be55-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0be55-111">payloadId</span><span class="sxs-lookup"><span data-stu-id="0be55-111">payloadId</span></span>|<span data-ttu-id="0be55-112">String</span><span class="sxs-lookup"><span data-stu-id="0be55-112">String</span></span>|<span data-ttu-id="0be55-113">有效负载的键，格式为 Guid。</span><span class="sxs-lookup"><span data-stu-id="0be55-113">Key of the Payload, In the format of Guid.</span></span>|
|<span data-ttu-id="0be55-114">hasLink</span><span class="sxs-lookup"><span data-stu-id="0be55-114">hasLink</span></span>|<span data-ttu-id="0be55-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="0be55-115">Boolean</span></span>|<span data-ttu-id="0be55-116">指示有效负载是否有任何链接。</span><span class="sxs-lookup"><span data-stu-id="0be55-116">Indicate whether a payload has any link or not.</span></span>|
|<span data-ttu-id="0be55-117">error</span><span class="sxs-lookup"><span data-stu-id="0be55-117">error</span></span>|<span data-ttu-id="0be55-118">String</span><span class="sxs-lookup"><span data-stu-id="0be55-118">String</span></span>|<span data-ttu-id="0be55-119">异常信息指示是否成功检查此项。空字符串表示无错误。</span><span class="sxs-lookup"><span data-stu-id="0be55-119">Exception information indicates if check for this item was successful or not.Empty string for no error.</span></span>|
|<span data-ttu-id="0be55-120">源</span><span class="sxs-lookup"><span data-stu-id="0be55-120">sources</span></span>|<span data-ttu-id="0be55-121">[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md)集合</span><span class="sxs-lookup"><span data-stu-id="0be55-121">[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md) collection</span></span>|<span data-ttu-id="0be55-122">链接来自的原因。</span><span class="sxs-lookup"><span data-stu-id="0be55-122">The reason where the link comes from.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0be55-123">关系</span><span class="sxs-lookup"><span data-stu-id="0be55-123">Relationships</span></span>
<span data-ttu-id="0be55-124">无</span><span class="sxs-lookup"><span data-stu-id="0be55-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0be55-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0be55-125">JSON Representation</span></span>
<span data-ttu-id="0be55-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0be55-126">Here is a JSON representation of the resource.</span></span>
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



