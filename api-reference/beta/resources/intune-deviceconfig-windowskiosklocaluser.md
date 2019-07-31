---
title: windowsKioskLocalUser 资源类型
description: 用于标识展台配置的本地帐户的类
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d3f46b47de9d3ce09c6a7d33a4b663cb64f506cc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969007"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="7a545-103">windowsKioskLocalUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="7a545-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="7a545-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7a545-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a545-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7a545-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a545-106">用于标识展台配置的本地帐户的类</span><span class="sxs-lookup"><span data-stu-id="7a545-106">The class used to identify a local account for the kiosk configuration</span></span>


<span data-ttu-id="7a545-107">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="7a545-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7a545-108">属性</span><span class="sxs-lookup"><span data-stu-id="7a545-108">Properties</span></span>
|<span data-ttu-id="7a545-109">属性</span><span class="sxs-lookup"><span data-stu-id="7a545-109">Property</span></span>|<span data-ttu-id="7a545-110">类型</span><span class="sxs-lookup"><span data-stu-id="7a545-110">Type</span></span>|<span data-ttu-id="7a545-111">说明</span><span class="sxs-lookup"><span data-stu-id="7a545-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a545-112">userName</span><span class="sxs-lookup"><span data-stu-id="7a545-112">userName</span></span>|<span data-ttu-id="7a545-113">String</span><span class="sxs-lookup"><span data-stu-id="7a545-113">String</span></span>|<span data-ttu-id="7a545-114">将锁定到此展台配置的本地用户</span><span class="sxs-lookup"><span data-stu-id="7a545-114">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a545-115">关系</span><span class="sxs-lookup"><span data-stu-id="7a545-115">Relationships</span></span>
<span data-ttu-id="7a545-116">无</span><span class="sxs-lookup"><span data-stu-id="7a545-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a545-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7a545-117">JSON Representation</span></span>
<span data-ttu-id="7a545-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7a545-118">Here is a JSON representation of the resource.</span></span>
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





