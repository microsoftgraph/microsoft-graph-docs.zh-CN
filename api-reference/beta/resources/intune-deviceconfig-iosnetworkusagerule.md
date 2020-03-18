---
title: iosNetworkUsageRule 资源类型
description: 网络使用规则允许企业指定托管应用使用网络的方式，例如手机数据网络。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 26e62ee0d470d178b15a849c16f4e1678cc0152e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790585"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="e1050-103">iosNetworkUsageRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1050-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="e1050-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e1050-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1050-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e1050-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1050-106">网络使用规则允许企业指定托管应用使用网络的方式，例如手机数据网络。</span><span class="sxs-lookup"><span data-stu-id="e1050-106">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="e1050-107">属性</span><span class="sxs-lookup"><span data-stu-id="e1050-107">Properties</span></span>
|<span data-ttu-id="e1050-108">属性</span><span class="sxs-lookup"><span data-stu-id="e1050-108">Property</span></span>|<span data-ttu-id="e1050-109">类型</span><span class="sxs-lookup"><span data-stu-id="e1050-109">Type</span></span>|<span data-ttu-id="e1050-110">说明</span><span class="sxs-lookup"><span data-stu-id="e1050-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1050-111">managedApps</span><span class="sxs-lookup"><span data-stu-id="e1050-111">managedApps</span></span>|<span data-ttu-id="e1050-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e1050-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="e1050-113">要应用此规则的托管应用的相关信息。</span><span class="sxs-lookup"><span data-stu-id="e1050-113">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="e1050-114">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="e1050-114">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="e1050-115">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="e1050-115">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="e1050-116">布尔值</span><span class="sxs-lookup"><span data-stu-id="e1050-116">Boolean</span></span>|<span data-ttu-id="e1050-117">如果设置为 true，则在漫游时将不允许相应的托管应用使用手机网络数据。</span><span class="sxs-lookup"><span data-stu-id="e1050-117">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="e1050-118">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="e1050-118">cellularDataBlocked</span></span>|<span data-ttu-id="e1050-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1050-119">Boolean</span></span>|<span data-ttu-id="e1050-120">如果设置为 true，则在任何时间均不允许相应的托管应用使用手机网络数据。</span><span class="sxs-lookup"><span data-stu-id="e1050-120">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1050-121">关系</span><span class="sxs-lookup"><span data-stu-id="e1050-121">Relationships</span></span>
<span data-ttu-id="e1050-122">无</span><span class="sxs-lookup"><span data-stu-id="e1050-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1050-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1050-123">JSON Representation</span></span>
<span data-ttu-id="e1050-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1050-124">Here is a JSON representation of the resource.</span></span>
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



