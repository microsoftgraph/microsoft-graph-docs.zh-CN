---
title: windowsKioskAzureADUser 资源类型
description: 用于为展台配置标识 AzureAD 用户帐户的类
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3dd72b65c8829f4b085d4bb8ec86c904746bf126
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000289"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="92dee-103">windowsKioskAzureADUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="92dee-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="92dee-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="92dee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92dee-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="92dee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92dee-106">用于为展台配置标识 AzureAD 用户帐户的类</span><span class="sxs-lookup"><span data-stu-id="92dee-106">The class used to identify an AzureAD user account for the kiosk configuration</span></span>


<span data-ttu-id="92dee-107">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="92dee-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="92dee-108">属性</span><span class="sxs-lookup"><span data-stu-id="92dee-108">Properties</span></span>
|<span data-ttu-id="92dee-109">属性</span><span class="sxs-lookup"><span data-stu-id="92dee-109">Property</span></span>|<span data-ttu-id="92dee-110">类型</span><span class="sxs-lookup"><span data-stu-id="92dee-110">Type</span></span>|<span data-ttu-id="92dee-111">说明</span><span class="sxs-lookup"><span data-stu-id="92dee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92dee-112">userId</span><span class="sxs-lookup"><span data-stu-id="92dee-112">userId</span></span>|<span data-ttu-id="92dee-113">String</span><span class="sxs-lookup"><span data-stu-id="92dee-113">String</span></span>|<span data-ttu-id="92dee-114">将锁定到此展台配置的 AzureAD 用户的 ID</span><span class="sxs-lookup"><span data-stu-id="92dee-114">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="92dee-115">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="92dee-115">userPrincipalName</span></span>|<span data-ttu-id="92dee-116">字符串</span><span class="sxs-lookup"><span data-stu-id="92dee-116">String</span></span>|<span data-ttu-id="92dee-117">将锁定到此展台配置的用户帐户</span><span class="sxs-lookup"><span data-stu-id="92dee-117">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="92dee-118">关系</span><span class="sxs-lookup"><span data-stu-id="92dee-118">Relationships</span></span>
<span data-ttu-id="92dee-119">无</span><span class="sxs-lookup"><span data-stu-id="92dee-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92dee-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="92dee-120">JSON Representation</span></span>
<span data-ttu-id="92dee-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92dee-121">Here is a JSON representation of the resource.</span></span>
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





