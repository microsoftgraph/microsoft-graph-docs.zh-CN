---
title: iosNetworkUsageRule 资源类型
description: 网络使用规则允许企业指定托管应用使用网络的方式，例如手机数据网络。
ms.openlocfilehash: 93cfd1f5eefe6f32fd0b112b24e3cdfba6969434
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045647"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="04fab-103">iosNetworkUsageRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="04fab-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="04fab-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="04fab-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04fab-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="04fab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04fab-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="04fab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04fab-107">网络使用规则允许企业指定托管应用使用网络的方式，例如手机数据网络。</span><span class="sxs-lookup"><span data-stu-id="04fab-107">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>
## <a name="properties"></a><span data-ttu-id="04fab-108">属性</span><span class="sxs-lookup"><span data-stu-id="04fab-108">Properties</span></span>
|<span data-ttu-id="04fab-109">属性</span><span class="sxs-lookup"><span data-stu-id="04fab-109">Property</span></span>|<span data-ttu-id="04fab-110">类型</span><span class="sxs-lookup"><span data-stu-id="04fab-110">Type</span></span>|<span data-ttu-id="04fab-111">说明</span><span class="sxs-lookup"><span data-stu-id="04fab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04fab-112">managedApps</span><span class="sxs-lookup"><span data-stu-id="04fab-112">managedApps</span></span>|<span data-ttu-id="04fab-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="04fab-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="04fab-114">要应用此规则的托管应用的相关信息。</span><span class="sxs-lookup"><span data-stu-id="04fab-114">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="04fab-115">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="04fab-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="04fab-116">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="04fab-116">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="04fab-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="04fab-117">Boolean</span></span>|<span data-ttu-id="04fab-118">如果设置为 true，则在漫游时将不允许相应的托管应用使用手机网络数据。</span><span class="sxs-lookup"><span data-stu-id="04fab-118">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="04fab-119">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="04fab-119">cellularDataBlocked</span></span>|<span data-ttu-id="04fab-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="04fab-120">Boolean</span></span>|<span data-ttu-id="04fab-121">如果设置为 true，则在任何时间均不允许相应的托管应用使用手机网络数据。</span><span class="sxs-lookup"><span data-stu-id="04fab-121">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04fab-122">关系</span><span class="sxs-lookup"><span data-stu-id="04fab-122">Relationships</span></span>
<span data-ttu-id="04fab-123">无</span><span class="sxs-lookup"><span data-stu-id="04fab-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="04fab-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04fab-124">JSON Representation</span></span>
<span data-ttu-id="04fab-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04fab-125">Here is a JSON representation of the resource.</span></span>
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





