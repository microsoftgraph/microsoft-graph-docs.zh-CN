---
title: iosNetworkUsageRule 资源类型
description: 网络使用规则允许企业指定托管应用使用网络的方式，例如手机数据网络。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0a287fcf8be771037a39efd821f5468acf518371
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398322"
---
# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="0e97c-103">iosNetworkUsageRule 资源类型</span><span class="sxs-lookup"><span data-stu-id="0e97c-103">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="0e97c-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="0e97c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0e97c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0e97c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e97c-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0e97c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e97c-107">网络使用规则允许企业指定托管应用使用网络的方式，例如手机数据网络。</span><span class="sxs-lookup"><span data-stu-id="0e97c-107">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>

## <a name="properties"></a><span data-ttu-id="0e97c-108">属性</span><span class="sxs-lookup"><span data-stu-id="0e97c-108">Properties</span></span>
|<span data-ttu-id="0e97c-109">属性</span><span class="sxs-lookup"><span data-stu-id="0e97c-109">Property</span></span>|<span data-ttu-id="0e97c-110">类型</span><span class="sxs-lookup"><span data-stu-id="0e97c-110">Type</span></span>|<span data-ttu-id="0e97c-111">说明</span><span class="sxs-lookup"><span data-stu-id="0e97c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e97c-112">managedApps</span><span class="sxs-lookup"><span data-stu-id="0e97c-112">managedApps</span></span>|<span data-ttu-id="0e97c-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0e97c-113">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="0e97c-114">要应用此规则的托管应用的相关信息。</span><span class="sxs-lookup"><span data-stu-id="0e97c-114">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="0e97c-115">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="0e97c-115">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="0e97c-116">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="0e97c-116">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="0e97c-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e97c-117">Boolean</span></span>|<span data-ttu-id="0e97c-118">如果设置为 true，则在漫游时将不允许相应的托管应用使用手机网络数据。</span><span class="sxs-lookup"><span data-stu-id="0e97c-118">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="0e97c-119">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="0e97c-119">cellularDataBlocked</span></span>|<span data-ttu-id="0e97c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="0e97c-120">Boolean</span></span>|<span data-ttu-id="0e97c-121">如果设置为 true，则在任何时间均不允许相应的托管应用使用手机网络数据。</span><span class="sxs-lookup"><span data-stu-id="0e97c-121">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e97c-122">关系</span><span class="sxs-lookup"><span data-stu-id="0e97c-122">Relationships</span></span>
<span data-ttu-id="0e97c-123">无</span><span class="sxs-lookup"><span data-stu-id="0e97c-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e97c-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e97c-124">JSON Representation</span></span>
<span data-ttu-id="0e97c-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e97c-125">Here is a JSON representation of the resource.</span></span>
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




