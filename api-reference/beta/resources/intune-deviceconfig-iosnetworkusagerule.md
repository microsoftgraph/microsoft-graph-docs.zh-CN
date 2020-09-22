---
title: iosNetworkUsageRule 资源类型
description: 网络使用规则允许企业指定托管应用使用网络的方式，例如手机数据网络。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f273ae6cd6d9b40dd19d65df342c0e83fef61bd5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085008"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="06afe-103">iosNetworkUsageRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="06afe-103">iosNetworkUsageRule resource type</span></span>

<span data-ttu-id="06afe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06afe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06afe-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="06afe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06afe-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06afe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06afe-107">网络使用规则允许企业指定托管应用使用网络的方式，例如手机数据网络。</span><span class="sxs-lookup"><span data-stu-id="06afe-107">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="06afe-108">属性</span><span class="sxs-lookup"><span data-stu-id="06afe-108">Properties</span></span>
|<span data-ttu-id="06afe-109">属性</span><span class="sxs-lookup"><span data-stu-id="06afe-109">Property</span></span>|<span data-ttu-id="06afe-110">类型</span><span class="sxs-lookup"><span data-stu-id="06afe-110">Type</span></span>|<span data-ttu-id="06afe-111">说明</span><span class="sxs-lookup"><span data-stu-id="06afe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06afe-112">managedApps</span><span class="sxs-lookup"><span data-stu-id="06afe-112">managedApps</span></span>|<span data-ttu-id="06afe-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06afe-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="06afe-114">要应用此规则的托管应用的相关信息。</span><span class="sxs-lookup"><span data-stu-id="06afe-114">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="06afe-115">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="06afe-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="06afe-116">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="06afe-116">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="06afe-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="06afe-117">Boolean</span></span>|<span data-ttu-id="06afe-118">如果设置为 true，则在漫游时将不允许相应的托管应用使用手机网络数据。</span><span class="sxs-lookup"><span data-stu-id="06afe-118">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="06afe-119">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="06afe-119">cellularDataBlocked</span></span>|<span data-ttu-id="06afe-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="06afe-120">Boolean</span></span>|<span data-ttu-id="06afe-121">如果设置为 true，则在任何时间均不允许相应的托管应用使用手机网络数据。</span><span class="sxs-lookup"><span data-stu-id="06afe-121">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06afe-122">关系</span><span class="sxs-lookup"><span data-stu-id="06afe-122">Relationships</span></span>
<span data-ttu-id="06afe-123">无</span><span class="sxs-lookup"><span data-stu-id="06afe-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06afe-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06afe-124">JSON Representation</span></span>
<span data-ttu-id="06afe-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06afe-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNetworkUsageRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNetworkUsageRule",
  "managedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "cellularDataBlockWhenRoaming": true,
  "cellularDataBlocked": true
}
```






