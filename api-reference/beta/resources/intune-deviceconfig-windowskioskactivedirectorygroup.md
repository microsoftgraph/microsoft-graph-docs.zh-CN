---
title: windowsKioskActiveDirectoryGroup 资源类型
description: 用于标识展台配置的 Azure 目录组的类
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e9f3345462583ab24850449d4a6178df7d5e3688
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147073"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="f3a29-103">windowsKioskActiveDirectoryGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="f3a29-103">windowsKioskActiveDirectoryGroup resource type</span></span>

> <span data-ttu-id="f3a29-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f3a29-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3a29-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f3a29-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3a29-106">用于标识展台配置的 Azure 目录组的类</span><span class="sxs-lookup"><span data-stu-id="f3a29-106">The class used to identify an Azure Directory group for the kiosk configuration</span></span>


<span data-ttu-id="f3a29-107">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="f3a29-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f3a29-108">属性</span><span class="sxs-lookup"><span data-stu-id="f3a29-108">Properties</span></span>
|<span data-ttu-id="f3a29-109">属性</span><span class="sxs-lookup"><span data-stu-id="f3a29-109">Property</span></span>|<span data-ttu-id="f3a29-110">类型</span><span class="sxs-lookup"><span data-stu-id="f3a29-110">Type</span></span>|<span data-ttu-id="f3a29-111">说明</span><span class="sxs-lookup"><span data-stu-id="f3a29-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3a29-112">名</span><span class="sxs-lookup"><span data-stu-id="f3a29-112">groupName</span></span>|<span data-ttu-id="f3a29-113">字符串</span><span class="sxs-lookup"><span data-stu-id="f3a29-113">String</span></span>|<span data-ttu-id="f3a29-114">将锁定到此展台配置的 AD 组的名称</span><span class="sxs-lookup"><span data-stu-id="f3a29-114">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3a29-115">关系</span><span class="sxs-lookup"><span data-stu-id="f3a29-115">Relationships</span></span>
<span data-ttu-id="f3a29-116">无</span><span class="sxs-lookup"><span data-stu-id="f3a29-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3a29-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f3a29-117">JSON Representation</span></span>
<span data-ttu-id="f3a29-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3a29-118">Here is a JSON representation of the resource.</span></span>
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




