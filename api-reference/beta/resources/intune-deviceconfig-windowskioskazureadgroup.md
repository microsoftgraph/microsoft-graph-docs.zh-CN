---
title: windowsKioskAzureADGroup 资源类型
description: 用于标识展台配置的 AzureAD 组的类
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a80ef23c94424b79d1392cd5632f8dce85f675d1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978518"
---
# <a name="windowskioskazureadgroup-resource-type"></a><span data-ttu-id="7c297-103">windowsKioskAzureADGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c297-103">windowsKioskAzureADGroup resource type</span></span>

> <span data-ttu-id="7c297-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7c297-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c297-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7c297-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c297-106">用于标识展台配置的 AzureAD 组的类</span><span class="sxs-lookup"><span data-stu-id="7c297-106">The class used to identify an AzureAD group for the kiosk configuration</span></span>


<span data-ttu-id="7c297-107">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="7c297-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7c297-108">属性</span><span class="sxs-lookup"><span data-stu-id="7c297-108">Properties</span></span>
|<span data-ttu-id="7c297-109">属性</span><span class="sxs-lookup"><span data-stu-id="7c297-109">Property</span></span>|<span data-ttu-id="7c297-110">类型</span><span class="sxs-lookup"><span data-stu-id="7c297-110">Type</span></span>|<span data-ttu-id="7c297-111">说明</span><span class="sxs-lookup"><span data-stu-id="7c297-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c297-112">displayName</span><span class="sxs-lookup"><span data-stu-id="7c297-112">displayName</span></span>|<span data-ttu-id="7c297-113">String</span><span class="sxs-lookup"><span data-stu-id="7c297-113">String</span></span>|<span data-ttu-id="7c297-114">将锁定到此展台配置的 AzureAD 组的显示名称</span><span class="sxs-lookup"><span data-stu-id="7c297-114">The display name of the AzureAD group that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="7c297-115">groupId</span><span class="sxs-lookup"><span data-stu-id="7c297-115">groupId</span></span>|<span data-ttu-id="7c297-116">String</span><span class="sxs-lookup"><span data-stu-id="7c297-116">String</span></span>|<span data-ttu-id="7c297-117">将锁定到此展台配置的 AzureAD 组的 ID</span><span class="sxs-lookup"><span data-stu-id="7c297-117">The ID of the AzureAD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="7c297-118">关系</span><span class="sxs-lookup"><span data-stu-id="7c297-118">Relationships</span></span>
<span data-ttu-id="7c297-119">无</span><span class="sxs-lookup"><span data-stu-id="7c297-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c297-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c297-120">JSON Representation</span></span>
<span data-ttu-id="7c297-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c297-121">Here is a JSON representation of the resource.</span></span>
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





