---
title: iosNetworkUsageRule 资源类型
description: 网络使用规则允许企业指定托管应用使用网络的方式，例如手机数据网络。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9e7315dfb5162694d48778f07650fb92bde9dfa8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760041"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="6d519-103">iosNetworkUsageRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="6d519-103">iosNetworkUsageRule resource type</span></span>

<span data-ttu-id="6d519-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d519-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d519-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6d519-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d519-106">网络使用规则允许企业指定托管应用使用网络的方式，例如手机数据网络。</span><span class="sxs-lookup"><span data-stu-id="6d519-106">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="6d519-107">属性</span><span class="sxs-lookup"><span data-stu-id="6d519-107">Properties</span></span>
|<span data-ttu-id="6d519-108">属性</span><span class="sxs-lookup"><span data-stu-id="6d519-108">Property</span></span>|<span data-ttu-id="6d519-109">类型</span><span class="sxs-lookup"><span data-stu-id="6d519-109">Type</span></span>|<span data-ttu-id="6d519-110">说明</span><span class="sxs-lookup"><span data-stu-id="6d519-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d519-111">managedApps</span><span class="sxs-lookup"><span data-stu-id="6d519-111">managedApps</span></span>|<span data-ttu-id="6d519-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6d519-112">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6d519-113">要应用此规则的托管应用的相关信息。</span><span class="sxs-lookup"><span data-stu-id="6d519-113">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="6d519-114">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="6d519-114">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6d519-115">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="6d519-115">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="6d519-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d519-116">Boolean</span></span>|<span data-ttu-id="6d519-117">如果设置为 true，则在漫游时将不允许相应的托管应用使用手机网络数据。</span><span class="sxs-lookup"><span data-stu-id="6d519-117">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="6d519-118">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="6d519-118">cellularDataBlocked</span></span>|<span data-ttu-id="6d519-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d519-119">Boolean</span></span>|<span data-ttu-id="6d519-120">如果设置为 true，则在任何时间均不允许相应的托管应用使用手机网络数据。</span><span class="sxs-lookup"><span data-stu-id="6d519-120">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d519-121">关系</span><span class="sxs-lookup"><span data-stu-id="6d519-121">Relationships</span></span>
<span data-ttu-id="6d519-122">无</span><span class="sxs-lookup"><span data-stu-id="6d519-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d519-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d519-123">JSON Representation</span></span>
<span data-ttu-id="6d519-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d519-124">Here is a JSON representation of the resource.</span></span>
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




