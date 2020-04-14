---
title: windowsKioskAzureADUser 资源类型
description: 用于为展台配置标识 AzureAD 用户帐户的类
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9c1dd759906ec4a4891fdbb2fb57d9c5258aa102
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466776"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="4ce23-103">windowsKioskAzureADUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="4ce23-103">windowsKioskAzureADUser resource type</span></span>

<span data-ttu-id="4ce23-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4ce23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ce23-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4ce23-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ce23-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4ce23-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ce23-107">用于为展台配置标识 AzureAD 用户帐户的类</span><span class="sxs-lookup"><span data-stu-id="4ce23-107">The class used to identify an AzureAD user account for the kiosk configuration</span></span>


<span data-ttu-id="4ce23-108">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="4ce23-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4ce23-109">属性</span><span class="sxs-lookup"><span data-stu-id="4ce23-109">Properties</span></span>
|<span data-ttu-id="4ce23-110">属性</span><span class="sxs-lookup"><span data-stu-id="4ce23-110">Property</span></span>|<span data-ttu-id="4ce23-111">类型</span><span class="sxs-lookup"><span data-stu-id="4ce23-111">Type</span></span>|<span data-ttu-id="4ce23-112">说明</span><span class="sxs-lookup"><span data-stu-id="4ce23-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ce23-113">userId</span><span class="sxs-lookup"><span data-stu-id="4ce23-113">userId</span></span>|<span data-ttu-id="4ce23-114">String</span><span class="sxs-lookup"><span data-stu-id="4ce23-114">String</span></span>|<span data-ttu-id="4ce23-115">将锁定到此展台配置的 AzureAD 用户的 ID</span><span class="sxs-lookup"><span data-stu-id="4ce23-115">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="4ce23-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4ce23-116">userPrincipalName</span></span>|<span data-ttu-id="4ce23-117">字符串</span><span class="sxs-lookup"><span data-stu-id="4ce23-117">String</span></span>|<span data-ttu-id="4ce23-118">将锁定到此展台配置的用户帐户</span><span class="sxs-lookup"><span data-stu-id="4ce23-118">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="4ce23-119">关系</span><span class="sxs-lookup"><span data-stu-id="4ce23-119">Relationships</span></span>
<span data-ttu-id="4ce23-120">无</span><span class="sxs-lookup"><span data-stu-id="4ce23-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ce23-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4ce23-121">JSON Representation</span></span>
<span data-ttu-id="4ce23-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ce23-122">Here is a JSON representation of the resource.</span></span>
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



