---
title: iosNetworkUsageRule 资源类型
description: 网络使用规则允许企业指定托管应用使用网络的方式，例如手机数据网络。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 84662ed78c4692bc64dd59f813dc1c056e8c0564
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36356926"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="6a189-103">iosNetworkUsageRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a189-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="6a189-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6a189-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a189-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6a189-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a189-106">网络使用规则允许企业指定托管应用使用网络的方式，例如手机数据网络。</span><span class="sxs-lookup"><span data-stu-id="6a189-106">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="6a189-107">属性</span><span class="sxs-lookup"><span data-stu-id="6a189-107">Properties</span></span>
|<span data-ttu-id="6a189-108">属性</span><span class="sxs-lookup"><span data-stu-id="6a189-108">Property</span></span>|<span data-ttu-id="6a189-109">类型</span><span class="sxs-lookup"><span data-stu-id="6a189-109">Type</span></span>|<span data-ttu-id="6a189-110">说明</span><span class="sxs-lookup"><span data-stu-id="6a189-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a189-111">managedApps</span><span class="sxs-lookup"><span data-stu-id="6a189-111">managedApps</span></span>|<span data-ttu-id="6a189-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6a189-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6a189-113">要应用此规则的托管应用的相关信息。</span><span class="sxs-lookup"><span data-stu-id="6a189-113">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="6a189-114">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6a189-114">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6a189-115">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="6a189-115">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="6a189-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a189-116">Boolean</span></span>|<span data-ttu-id="6a189-117">如果设置为 true，则在漫游时将不允许相应的托管应用使用手机网络数据。</span><span class="sxs-lookup"><span data-stu-id="6a189-117">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="6a189-118">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="6a189-118">cellularDataBlocked</span></span>|<span data-ttu-id="6a189-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a189-119">Boolean</span></span>|<span data-ttu-id="6a189-120">如果设置为 true，则在任何时间均不允许相应的托管应用使用手机网络数据。</span><span class="sxs-lookup"><span data-stu-id="6a189-120">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a189-121">关系</span><span class="sxs-lookup"><span data-stu-id="6a189-121">Relationships</span></span>
<span data-ttu-id="6a189-122">无</span><span class="sxs-lookup"><span data-stu-id="6a189-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a189-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a189-123">JSON Representation</span></span>
<span data-ttu-id="6a189-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a189-124">Here is a JSON representation of the resource.</span></span>
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



