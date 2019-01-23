---
title: windowsKioskAzureADUser 资源类型
description: 用于标识网亭配置 AzureAD 用户帐户的类
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 08c5b53e8e208abac2801146ff70df6023eaedff
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420183"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="cffca-103">windowsKioskAzureADUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="cffca-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="cffca-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="cffca-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cffca-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cffca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cffca-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cffca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cffca-107">用于标识网亭配置 AzureAD 用户帐户的类</span><span class="sxs-lookup"><span data-stu-id="cffca-107">The class used to identify an AzureAD user account for the kiosk configuration</span></span>


<span data-ttu-id="cffca-108">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="cffca-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="cffca-109">属性</span><span class="sxs-lookup"><span data-stu-id="cffca-109">Properties</span></span>
|<span data-ttu-id="cffca-110">属性</span><span class="sxs-lookup"><span data-stu-id="cffca-110">Property</span></span>|<span data-ttu-id="cffca-111">类型</span><span class="sxs-lookup"><span data-stu-id="cffca-111">Type</span></span>|<span data-ttu-id="cffca-112">说明</span><span class="sxs-lookup"><span data-stu-id="cffca-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cffca-113">userId</span><span class="sxs-lookup"><span data-stu-id="cffca-113">userId</span></span>|<span data-ttu-id="cffca-114">String</span><span class="sxs-lookup"><span data-stu-id="cffca-114">String</span></span>|<span data-ttu-id="cffca-115">将锁定到此网亭配置 AzureAD 用户的 ID</span><span class="sxs-lookup"><span data-stu-id="cffca-115">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="cffca-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cffca-116">userPrincipalName</span></span>|<span data-ttu-id="cffca-117">String</span><span class="sxs-lookup"><span data-stu-id="cffca-117">String</span></span>|<span data-ttu-id="cffca-118">将锁定到此网亭配置用户帐户</span><span class="sxs-lookup"><span data-stu-id="cffca-118">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="cffca-119">关系</span><span class="sxs-lookup"><span data-stu-id="cffca-119">Relationships</span></span>
<span data-ttu-id="cffca-120">无</span><span class="sxs-lookup"><span data-stu-id="cffca-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cffca-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cffca-121">JSON Representation</span></span>
<span data-ttu-id="cffca-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cffca-122">Here is a JSON representation of the resource.</span></span>
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




