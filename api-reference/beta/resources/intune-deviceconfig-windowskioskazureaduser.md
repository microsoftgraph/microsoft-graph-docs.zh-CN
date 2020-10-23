---
title: windowsKioskAzureADUser 资源类型
description: 用于为展台配置标识 AzureAD 用户帐户的类
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4b946007fd8b16d2f6c016025d58e07392b6c1a9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48690656"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="92095-103">windowsKioskAzureADUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="92095-103">windowsKioskAzureADUser resource type</span></span>

<span data-ttu-id="92095-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="92095-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="92095-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="92095-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92095-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="92095-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92095-107">用于为展台配置标识 AzureAD 用户帐户的类</span><span class="sxs-lookup"><span data-stu-id="92095-107">The class used to identify an AzureAD user account for the kiosk configuration</span></span>


<span data-ttu-id="92095-108">继承自 [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="92095-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="92095-109">属性</span><span class="sxs-lookup"><span data-stu-id="92095-109">Properties</span></span>
|<span data-ttu-id="92095-110">属性</span><span class="sxs-lookup"><span data-stu-id="92095-110">Property</span></span>|<span data-ttu-id="92095-111">类型</span><span class="sxs-lookup"><span data-stu-id="92095-111">Type</span></span>|<span data-ttu-id="92095-112">描述</span><span class="sxs-lookup"><span data-stu-id="92095-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92095-113">userId</span><span class="sxs-lookup"><span data-stu-id="92095-113">userId</span></span>|<span data-ttu-id="92095-114">String</span><span class="sxs-lookup"><span data-stu-id="92095-114">String</span></span>|<span data-ttu-id="92095-115">将锁定到此展台配置的 AzureAD 用户的 ID</span><span class="sxs-lookup"><span data-stu-id="92095-115">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="92095-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="92095-116">userPrincipalName</span></span>|<span data-ttu-id="92095-117">String</span><span class="sxs-lookup"><span data-stu-id="92095-117">String</span></span>|<span data-ttu-id="92095-118">将锁定到此展台配置的用户帐户</span><span class="sxs-lookup"><span data-stu-id="92095-118">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="92095-119">关系</span><span class="sxs-lookup"><span data-stu-id="92095-119">Relationships</span></span>
<span data-ttu-id="92095-120">无</span><span class="sxs-lookup"><span data-stu-id="92095-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92095-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92095-121">JSON Representation</span></span>
<span data-ttu-id="92095-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92095-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADUser",
  "userId": "String",
  "userPrincipalName": "String"
}
```





