---
title: windowsKioskAzureADGroup 资源类型
description: 用于标识为网亭配置 AzureAD 组的类
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d4c8e0867346253c6501ebe8be490ba56800ab3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392568"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="79a1e-103">windowsKioskAzureADGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="79a1e-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="79a1e-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="79a1e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="79a1e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="79a1e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79a1e-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="79a1e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79a1e-107">用于标识为网亭配置 AzureAD 组的类</span><span class="sxs-lookup"><span data-stu-id="79a1e-107">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="79a1e-108">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="79a1e-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="79a1e-109">属性</span><span class="sxs-lookup"><span data-stu-id="79a1e-109">Properties</span></span>
|<span data-ttu-id="79a1e-110">属性</span><span class="sxs-lookup"><span data-stu-id="79a1e-110">Property</span></span>|<span data-ttu-id="79a1e-111">类型</span><span class="sxs-lookup"><span data-stu-id="79a1e-111">Type</span></span>|<span data-ttu-id="79a1e-112">说明</span><span class="sxs-lookup"><span data-stu-id="79a1e-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79a1e-113">displayName</span><span class="sxs-lookup"><span data-stu-id="79a1e-113">displayName</span></span>|<span data-ttu-id="79a1e-114">String</span><span class="sxs-lookup"><span data-stu-id="79a1e-114">String</span></span>|<span data-ttu-id="79a1e-115">将锁定到此网亭配置 AzureAD 组的显示名称</span><span class="sxs-lookup"><span data-stu-id="79a1e-115">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="79a1e-116">groupId</span><span class="sxs-lookup"><span data-stu-id="79a1e-116">groupId</span></span>|<span data-ttu-id="79a1e-117">String</span><span class="sxs-lookup"><span data-stu-id="79a1e-117">String</span></span>|<span data-ttu-id="79a1e-118">将此网亭配置到锁定的 AzureAD 组 ID</span><span class="sxs-lookup"><span data-stu-id="79a1e-118">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="79a1e-119">关系</span><span class="sxs-lookup"><span data-stu-id="79a1e-119">Relationships</span></span>
<span data-ttu-id="79a1e-120">无</span><span class="sxs-lookup"><span data-stu-id="79a1e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79a1e-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="79a1e-121">JSON Representation</span></span>
<span data-ttu-id="79a1e-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79a1e-122">Here is a JSON representation of the resource.</span></span>
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




