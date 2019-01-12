---
title: windowsKioskAzureADUser 资源类型
description: 用于标识网亭配置 AzureAD 用户帐户的类
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4497c6d42db45f518e3ef93e78e50d25f473ac00
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984141"
---
# <a name="windowskioskazureaduser-resource-type"></a><span data-ttu-id="c11e2-103">windowsKioskAzureADUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="c11e2-103">windowsKioskAzureADUser resource type</span></span>

> <span data-ttu-id="c11e2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c11e2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c11e2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c11e2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c11e2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c11e2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c11e2-107">用于标识网亭配置 AzureAD 用户帐户的类</span><span class="sxs-lookup"><span data-stu-id="c11e2-107">The class used to identify an AzureAD user account for the kiosk configuration</span></span>

<span data-ttu-id="c11e2-108">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="c11e2-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c11e2-109">属性</span><span class="sxs-lookup"><span data-stu-id="c11e2-109">Properties</span></span>
|<span data-ttu-id="c11e2-110">属性</span><span class="sxs-lookup"><span data-stu-id="c11e2-110">Property</span></span>|<span data-ttu-id="c11e2-111">类型</span><span class="sxs-lookup"><span data-stu-id="c11e2-111">Type</span></span>|<span data-ttu-id="c11e2-112">说明</span><span class="sxs-lookup"><span data-stu-id="c11e2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c11e2-113">userId</span><span class="sxs-lookup"><span data-stu-id="c11e2-113">userId</span></span>|<span data-ttu-id="c11e2-114">String</span><span class="sxs-lookup"><span data-stu-id="c11e2-114">String</span></span>|<span data-ttu-id="c11e2-115">将锁定到此网亭配置 AzureAD 用户的 ID</span><span class="sxs-lookup"><span data-stu-id="c11e2-115">The ID of the AzureAD user that will be locked to this kiosk configuration</span></span>|
|<span data-ttu-id="c11e2-116">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c11e2-116">userPrincipalName</span></span>|<span data-ttu-id="c11e2-117">字符串</span><span class="sxs-lookup"><span data-stu-id="c11e2-117">String</span></span>|<span data-ttu-id="c11e2-118">将锁定到此网亭配置用户帐户</span><span class="sxs-lookup"><span data-stu-id="c11e2-118">The user accounts that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="c11e2-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="c11e2-119">Relationships</span></span>
<span data-ttu-id="c11e2-120">无</span><span class="sxs-lookup"><span data-stu-id="c11e2-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c11e2-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c11e2-121">JSON Representation</span></span>
<span data-ttu-id="c11e2-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c11e2-122">Here is a JSON representation of the resource.</span></span>
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





