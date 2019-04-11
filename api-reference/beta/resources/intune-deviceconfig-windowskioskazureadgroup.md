---
title: windowsKioskAzureADGroup 资源类型
description: 用于标识展台配置的 AzureAD 组的类
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a3224f55f4a5158fb8c0850a4dbea7e6bcf8d18d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31778052"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="6ec42-103">windowsKioskAzureADGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="6ec42-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="6ec42-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6ec42-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ec42-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6ec42-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ec42-106">用于标识展台配置的 AzureAD 组的类</span><span class="sxs-lookup"><span data-stu-id="6ec42-106">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="6ec42-107">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="6ec42-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="6ec42-108">属性</span><span class="sxs-lookup"><span data-stu-id="6ec42-108">Properties</span></span>
|<span data-ttu-id="6ec42-109">属性</span><span class="sxs-lookup"><span data-stu-id="6ec42-109">Property</span></span>|<span data-ttu-id="6ec42-110">类型</span><span class="sxs-lookup"><span data-stu-id="6ec42-110">Type</span></span>|<span data-ttu-id="6ec42-111">说明</span><span class="sxs-lookup"><span data-stu-id="6ec42-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ec42-112">displayName</span><span class="sxs-lookup"><span data-stu-id="6ec42-112">displayName</span></span>|<span data-ttu-id="6ec42-113">String</span><span class="sxs-lookup"><span data-stu-id="6ec42-113">String</span></span>|<span data-ttu-id="6ec42-114">将锁定到此展台配置的 AzureAD 组的显示名称</span><span class="sxs-lookup"><span data-stu-id="6ec42-114">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="6ec42-115">groupId</span><span class="sxs-lookup"><span data-stu-id="6ec42-115">groupId</span></span>|<span data-ttu-id="6ec42-116">String</span><span class="sxs-lookup"><span data-stu-id="6ec42-116">String</span></span>|<span data-ttu-id="6ec42-117">将锁定到此展台配置的 AzureAD 组的 ID</span><span class="sxs-lookup"><span data-stu-id="6ec42-117">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ec42-118">关系</span><span class="sxs-lookup"><span data-stu-id="6ec42-118">Relationships</span></span>
<span data-ttu-id="6ec42-119">无</span><span class="sxs-lookup"><span data-stu-id="6ec42-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ec42-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ec42-120">JSON Representation</span></span>
<span data-ttu-id="6ec42-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ec42-121">Here is a JSON representation of the resource.</span></span>
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





