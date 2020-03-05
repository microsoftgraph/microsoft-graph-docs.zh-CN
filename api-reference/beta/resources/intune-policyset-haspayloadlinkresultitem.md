---
title: hasPayloadLinkResultItem 资源类型
description: 包含 HasPayloadLinks 操作结果的类。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 219bf9b1a2058b06895ec90883849cc8bdf0b569
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524004"
---
# <a name="haspayloadlinkresultitem-resource-type"></a><span data-ttu-id="c7e8d-103">hasPayloadLinkResultItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="c7e8d-103">hasPayloadLinkResultItem resource type</span></span>

<span data-ttu-id="c7e8d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c7e8d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c7e8d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c7e8d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c7e8d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c7e8d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c7e8d-107">包含 HasPayloadLinks 操作结果的类。</span><span class="sxs-lookup"><span data-stu-id="c7e8d-107">A class containing the result of HasPayloadLinks action.</span></span>

## <a name="properties"></a><span data-ttu-id="c7e8d-108">属性</span><span class="sxs-lookup"><span data-stu-id="c7e8d-108">Properties</span></span>
|<span data-ttu-id="c7e8d-109">属性</span><span class="sxs-lookup"><span data-stu-id="c7e8d-109">Property</span></span>|<span data-ttu-id="c7e8d-110">类型</span><span class="sxs-lookup"><span data-stu-id="c7e8d-110">Type</span></span>|<span data-ttu-id="c7e8d-111">说明</span><span class="sxs-lookup"><span data-stu-id="c7e8d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c7e8d-112">payloadId</span><span class="sxs-lookup"><span data-stu-id="c7e8d-112">payloadId</span></span>|<span data-ttu-id="c7e8d-113">String</span><span class="sxs-lookup"><span data-stu-id="c7e8d-113">String</span></span>|<span data-ttu-id="c7e8d-114">有效负载的键，格式为 Guid。</span><span class="sxs-lookup"><span data-stu-id="c7e8d-114">Key of the Payload, In the format of Guid.</span></span>|
|<span data-ttu-id="c7e8d-115">hasLink</span><span class="sxs-lookup"><span data-stu-id="c7e8d-115">hasLink</span></span>|<span data-ttu-id="c7e8d-116">布尔</span><span class="sxs-lookup"><span data-stu-id="c7e8d-116">Boolean</span></span>|<span data-ttu-id="c7e8d-117">指示有效负载是否有任何链接。</span><span class="sxs-lookup"><span data-stu-id="c7e8d-117">Indicate whether a payload has any link or not.</span></span>|
|<span data-ttu-id="c7e8d-118">error</span><span class="sxs-lookup"><span data-stu-id="c7e8d-118">error</span></span>|<span data-ttu-id="c7e8d-119">String</span><span class="sxs-lookup"><span data-stu-id="c7e8d-119">String</span></span>|<span data-ttu-id="c7e8d-120">异常信息指示是否成功检查此项。空字符串表示无错误。</span><span class="sxs-lookup"><span data-stu-id="c7e8d-120">Exception information indicates if check for this item was successful or not.Empty string for no error.</span></span>|
|<span data-ttu-id="c7e8d-121">源</span><span class="sxs-lookup"><span data-stu-id="c7e8d-121">sources</span></span>|<span data-ttu-id="c7e8d-122">[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md)集合</span><span class="sxs-lookup"><span data-stu-id="c7e8d-122">[deviceAndAppManagementAssignmentSource](../resources/intune-shared-deviceandappmanagementassignmentsource.md) collection</span></span>|<span data-ttu-id="c7e8d-123">链接来自的原因。</span><span class="sxs-lookup"><span data-stu-id="c7e8d-123">The reason where the link comes from.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c7e8d-124">关系</span><span class="sxs-lookup"><span data-stu-id="c7e8d-124">Relationships</span></span>
<span data-ttu-id="c7e8d-125">无</span><span class="sxs-lookup"><span data-stu-id="c7e8d-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c7e8d-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c7e8d-126">JSON Representation</span></span>
<span data-ttu-id="c7e8d-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c7e8d-127">Here is a JSON representation of the resource.</span></span>
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



