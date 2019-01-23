---
title: windowsKioskLocalUser 资源类型
description: 用于标识网亭配置的本地帐户的类
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b808cdb6cb8bb8540a553104d2c00108341a3e14
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29392666"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="1e878-103">windowsKioskLocalUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="1e878-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="1e878-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="1e878-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1e878-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1e878-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1e878-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1e878-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e878-107">用于标识网亭配置的本地帐户的类</span><span class="sxs-lookup"><span data-stu-id="1e878-107">The class used to identify a local account for the kiosk configuration</span></span>


<span data-ttu-id="1e878-108">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="1e878-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1e878-109">属性</span><span class="sxs-lookup"><span data-stu-id="1e878-109">Properties</span></span>
|<span data-ttu-id="1e878-110">属性</span><span class="sxs-lookup"><span data-stu-id="1e878-110">Property</span></span>|<span data-ttu-id="1e878-111">类型</span><span class="sxs-lookup"><span data-stu-id="1e878-111">Type</span></span>|<span data-ttu-id="1e878-112">说明</span><span class="sxs-lookup"><span data-stu-id="1e878-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e878-113">userName</span><span class="sxs-lookup"><span data-stu-id="1e878-113">userName</span></span>|<span data-ttu-id="1e878-114">String</span><span class="sxs-lookup"><span data-stu-id="1e878-114">String</span></span>|<span data-ttu-id="1e878-115">将锁定到此网亭配置本地用户</span><span class="sxs-lookup"><span data-stu-id="1e878-115">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e878-116">关系</span><span class="sxs-lookup"><span data-stu-id="1e878-116">Relationships</span></span>
<span data-ttu-id="1e878-117">无</span><span class="sxs-lookup"><span data-stu-id="1e878-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e878-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1e878-118">JSON Representation</span></span>
<span data-ttu-id="1e878-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e878-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalUser",
  "userName": "String"
}
```




