---
title: iosNetworkUsageRule 资源类型
description: 网络使用规则允许企业指定托管应用使用网络的方式，例如手机数据网络。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: abe641a0a714c8e2d9e171ccb874905b3a6321b6
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359059"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="f987e-103">iosNetworkUsageRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="f987e-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="f987e-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f987e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f987e-105">网络使用规则允许企业指定托管应用使用网络的方式，例如手机数据网络。</span><span class="sxs-lookup"><span data-stu-id="f987e-105">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="f987e-106">属性</span><span class="sxs-lookup"><span data-stu-id="f987e-106">Properties</span></span>
|<span data-ttu-id="f987e-107">属性</span><span class="sxs-lookup"><span data-stu-id="f987e-107">Property</span></span>|<span data-ttu-id="f987e-108">类型</span><span class="sxs-lookup"><span data-stu-id="f987e-108">Type</span></span>|<span data-ttu-id="f987e-109">说明</span><span class="sxs-lookup"><span data-stu-id="f987e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f987e-110">managedApps</span><span class="sxs-lookup"><span data-stu-id="f987e-110">managedApps</span></span>|<span data-ttu-id="f987e-111">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f987e-111">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f987e-112">要应用此规则的托管应用的相关信息。</span><span class="sxs-lookup"><span data-stu-id="f987e-112">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="f987e-113">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="f987e-113">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f987e-114">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="f987e-114">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="f987e-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="f987e-115">Boolean</span></span>|<span data-ttu-id="f987e-116">如果设置为 true，则在漫游时将不允许相应的托管应用使用手机网络数据。</span><span class="sxs-lookup"><span data-stu-id="f987e-116">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="f987e-117">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="f987e-117">cellularDataBlocked</span></span>|<span data-ttu-id="f987e-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="f987e-118">Boolean</span></span>|<span data-ttu-id="f987e-119">如果设置为 true，则在任何时间均不允许相应的托管应用使用手机网络数据。</span><span class="sxs-lookup"><span data-stu-id="f987e-119">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f987e-120">关系</span><span class="sxs-lookup"><span data-stu-id="f987e-120">Relationships</span></span>
<span data-ttu-id="f987e-121">无</span><span class="sxs-lookup"><span data-stu-id="f987e-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f987e-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f987e-122">JSON Representation</span></span>
<span data-ttu-id="f987e-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f987e-123">Here is a JSON representation of the resource.</span></span>
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




