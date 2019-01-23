---
title: windowsKioskActiveDirectoryGroup 资源类型
description: 用于标识为网亭配置 Azure Directory 组的类
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 88b151b856809247cfa6e5e211cc45c6f33c4c53
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415710"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="fccd4-103">windowsKioskActiveDirectoryGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="fccd4-103">windowsKioskActiveDirectoryGroup resource type</span></span>

> <span data-ttu-id="fccd4-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="fccd4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fccd4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fccd4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fccd4-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fccd4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fccd4-107">用于标识为网亭配置 Azure Directory 组的类</span><span class="sxs-lookup"><span data-stu-id="fccd4-107">The class used to identify an Azure Directory group for the kiosk configuration</span></span>


<span data-ttu-id="fccd4-108">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="fccd4-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fccd4-109">属性</span><span class="sxs-lookup"><span data-stu-id="fccd4-109">Properties</span></span>
|<span data-ttu-id="fccd4-110">属性</span><span class="sxs-lookup"><span data-stu-id="fccd4-110">Property</span></span>|<span data-ttu-id="fccd4-111">类型</span><span class="sxs-lookup"><span data-stu-id="fccd4-111">Type</span></span>|<span data-ttu-id="fccd4-112">说明</span><span class="sxs-lookup"><span data-stu-id="fccd4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fccd4-113">groupName</span><span class="sxs-lookup"><span data-stu-id="fccd4-113">groupName</span></span>|<span data-ttu-id="fccd4-114">String</span><span class="sxs-lookup"><span data-stu-id="fccd4-114">String</span></span>|<span data-ttu-id="fccd4-115">将锁定到此网亭配置 AD 组的名称</span><span class="sxs-lookup"><span data-stu-id="fccd4-115">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="fccd4-116">关系</span><span class="sxs-lookup"><span data-stu-id="fccd4-116">Relationships</span></span>
<span data-ttu-id="fccd4-117">无</span><span class="sxs-lookup"><span data-stu-id="fccd4-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fccd4-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fccd4-118">JSON Representation</span></span>
<span data-ttu-id="fccd4-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fccd4-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskActiveDirectoryGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskActiveDirectoryGroup",
  "groupName": "String"
}
```




