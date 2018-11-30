---
title: iosNetworkUsageRule 资源类型
description: 网络使用规则允许企业指定托管应用使用网络的方式，例如手机数据网络。
ms.openlocfilehash: 211cbc52f596bbe62647a14c84bd5fd5178fdfc6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011384"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="f7cdb-103">iosNetworkUsageRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7cdb-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="f7cdb-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f7cdb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7cdb-105">网络使用规则允许企业指定托管应用使用网络的方式，例如手机数据网络。</span><span class="sxs-lookup"><span data-stu-id="f7cdb-105">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>
## <a name="properties"></a><span data-ttu-id="f7cdb-106">属性</span><span class="sxs-lookup"><span data-stu-id="f7cdb-106">Properties</span></span>
|<span data-ttu-id="f7cdb-107">属性</span><span class="sxs-lookup"><span data-stu-id="f7cdb-107">Property</span></span>|<span data-ttu-id="f7cdb-108">类型</span><span class="sxs-lookup"><span data-stu-id="f7cdb-108">Type</span></span>|<span data-ttu-id="f7cdb-109">说明</span><span class="sxs-lookup"><span data-stu-id="f7cdb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7cdb-110">managedApps</span><span class="sxs-lookup"><span data-stu-id="f7cdb-110">managedApps</span></span>|<span data-ttu-id="f7cdb-111">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f7cdb-111">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f7cdb-112">要应用此规则的托管应用的相关信息。</span><span class="sxs-lookup"><span data-stu-id="f7cdb-112">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="f7cdb-113">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="f7cdb-113">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f7cdb-114">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="f7cdb-114">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="f7cdb-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7cdb-115">Boolean</span></span>|<span data-ttu-id="f7cdb-116">如果设置为 true，则在漫游时将不允许相应的托管应用使用手机网络数据。</span><span class="sxs-lookup"><span data-stu-id="f7cdb-116">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="f7cdb-117">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="f7cdb-117">cellularDataBlocked</span></span>|<span data-ttu-id="f7cdb-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="f7cdb-118">Boolean</span></span>|<span data-ttu-id="f7cdb-119">如果设置为 true，则在任何时间均不允许相应的托管应用使用手机网络数据。</span><span class="sxs-lookup"><span data-stu-id="f7cdb-119">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7cdb-120">关系</span><span class="sxs-lookup"><span data-stu-id="f7cdb-120">Relationships</span></span>
<span data-ttu-id="f7cdb-121">无</span><span class="sxs-lookup"><span data-stu-id="f7cdb-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f7cdb-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7cdb-122">JSON Representation</span></span>
<span data-ttu-id="f7cdb-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7cdb-123">Here is a JSON representation of the resource.</span></span>
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



