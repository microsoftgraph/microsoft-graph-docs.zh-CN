---
title: windowsKioskActiveDirectoryGroup 资源类型
description: 用于标识展台配置的 Azure 目录组的类
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4c0810cfeda4f620f6733a5b824cde8d0234f38
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943961"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="110e0-103">windowsKioskActiveDirectoryGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="110e0-103">windowsKioskActiveDirectoryGroup resource type</span></span>

> <span data-ttu-id="110e0-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="110e0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="110e0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="110e0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="110e0-106">用于标识展台配置的 Azure 目录组的类</span><span class="sxs-lookup"><span data-stu-id="110e0-106">The class used to identify an Azure Directory group for the kiosk configuration</span></span>


<span data-ttu-id="110e0-107">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="110e0-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="110e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="110e0-108">Properties</span></span>
|<span data-ttu-id="110e0-109">属性</span><span class="sxs-lookup"><span data-stu-id="110e0-109">Property</span></span>|<span data-ttu-id="110e0-110">类型</span><span class="sxs-lookup"><span data-stu-id="110e0-110">Type</span></span>|<span data-ttu-id="110e0-111">说明</span><span class="sxs-lookup"><span data-stu-id="110e0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="110e0-112">名</span><span class="sxs-lookup"><span data-stu-id="110e0-112">groupName</span></span>|<span data-ttu-id="110e0-113">String</span><span class="sxs-lookup"><span data-stu-id="110e0-113">String</span></span>|<span data-ttu-id="110e0-114">将锁定到此展台配置的 AD 组的名称</span><span class="sxs-lookup"><span data-stu-id="110e0-114">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="110e0-115">关系</span><span class="sxs-lookup"><span data-stu-id="110e0-115">Relationships</span></span>
<span data-ttu-id="110e0-116">无</span><span class="sxs-lookup"><span data-stu-id="110e0-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="110e0-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="110e0-117">JSON Representation</span></span>
<span data-ttu-id="110e0-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="110e0-118">Here is a JSON representation of the resource.</span></span>
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




