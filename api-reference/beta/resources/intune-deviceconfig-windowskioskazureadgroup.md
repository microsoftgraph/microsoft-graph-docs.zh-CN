---
title: windowsKioskAzureADGroup 资源类型
description: 用于标识展台配置的 AzureAD 组的类
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6569dc23786b9587ab7290859ff9a151a3e370c2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525507"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="6e5a7-103">windowsKioskAzureADGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="6e5a7-103">windowsKioskAzureADGroup resource type</span></span>

<span data-ttu-id="6e5a7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6e5a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e5a7-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6e5a7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e5a7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6e5a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e5a7-107">用于标识展台配置的 AzureAD 组的类</span><span class="sxs-lookup"><span data-stu-id="6e5a7-107">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="6e5a7-108">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="6e5a7-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6e5a7-109">属性</span><span class="sxs-lookup"><span data-stu-id="6e5a7-109">Properties</span></span>
|<span data-ttu-id="6e5a7-110">属性</span><span class="sxs-lookup"><span data-stu-id="6e5a7-110">Property</span></span>|<span data-ttu-id="6e5a7-111">类型</span><span class="sxs-lookup"><span data-stu-id="6e5a7-111">Type</span></span>|<span data-ttu-id="6e5a7-112">说明</span><span class="sxs-lookup"><span data-stu-id="6e5a7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e5a7-113">displayName</span><span class="sxs-lookup"><span data-stu-id="6e5a7-113">displayName</span></span>|<span data-ttu-id="6e5a7-114">String</span><span class="sxs-lookup"><span data-stu-id="6e5a7-114">String</span></span>|<span data-ttu-id="6e5a7-115">将锁定到此展台配置的 AzureAD 组的显示名称</span><span class="sxs-lookup"><span data-stu-id="6e5a7-115">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="6e5a7-116">groupId</span><span class="sxs-lookup"><span data-stu-id="6e5a7-116">groupId</span></span>|<span data-ttu-id="6e5a7-117">String</span><span class="sxs-lookup"><span data-stu-id="6e5a7-117">String</span></span>|<span data-ttu-id="6e5a7-118">将锁定到此展台配置的 AzureAD 组的 ID</span><span class="sxs-lookup"><span data-stu-id="6e5a7-118">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e5a7-119">关系</span><span class="sxs-lookup"><span data-stu-id="6e5a7-119">Relationships</span></span>
<span data-ttu-id="6e5a7-120">无</span><span class="sxs-lookup"><span data-stu-id="6e5a7-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e5a7-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6e5a7-121">JSON Representation</span></span>
<span data-ttu-id="6e5a7-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6e5a7-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADGroup",
  "displayName": "String",
  "groupId": "String"
}
```



