---
title: windowsKioskLocalUser 资源类型
description: 用于标识展台配置的本地帐户的类
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a84b1d3ce0a6e0f9de0bf60de314c79c0a7b329
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786374"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="faa70-103">windowsKioskLocalUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="faa70-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="faa70-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="faa70-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="faa70-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="faa70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faa70-106">用于标识展台配置的本地帐户的类</span><span class="sxs-lookup"><span data-stu-id="faa70-106">The class used to identify a local account for the kiosk configuration</span></span>


<span data-ttu-id="faa70-107">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="faa70-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="faa70-108">属性</span><span class="sxs-lookup"><span data-stu-id="faa70-108">Properties</span></span>
|<span data-ttu-id="faa70-109">属性</span><span class="sxs-lookup"><span data-stu-id="faa70-109">Property</span></span>|<span data-ttu-id="faa70-110">类型</span><span class="sxs-lookup"><span data-stu-id="faa70-110">Type</span></span>|<span data-ttu-id="faa70-111">说明</span><span class="sxs-lookup"><span data-stu-id="faa70-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faa70-112">userName</span><span class="sxs-lookup"><span data-stu-id="faa70-112">userName</span></span>|<span data-ttu-id="faa70-113">String</span><span class="sxs-lookup"><span data-stu-id="faa70-113">String</span></span>|<span data-ttu-id="faa70-114">将锁定到此展台配置的本地用户</span><span class="sxs-lookup"><span data-stu-id="faa70-114">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="faa70-115">关系</span><span class="sxs-lookup"><span data-stu-id="faa70-115">Relationships</span></span>
<span data-ttu-id="faa70-116">无</span><span class="sxs-lookup"><span data-stu-id="faa70-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="faa70-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="faa70-117">JSON Representation</span></span>
<span data-ttu-id="faa70-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="faa70-118">Here is a JSON representation of the resource.</span></span>
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



