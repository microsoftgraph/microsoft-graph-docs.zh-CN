---
title: windowsKioskActiveDirectoryGroup 资源类型
description: 用于标识展台配置的 Azure 目录组的类
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ab2a9834e4f3eac6fbff84fc84a78873aca8415f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529058"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="f5ee2-103">windowsKioskActiveDirectoryGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="f5ee2-103">windowsKioskActiveDirectoryGroup resource type</span></span>

<span data-ttu-id="f5ee2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f5ee2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5ee2-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5ee2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5ee2-107">用于标识展台配置的 Azure 目录组的类</span><span class="sxs-lookup"><span data-stu-id="f5ee2-107">The class used to identify an Azure Directory group for the kiosk configuration</span></span>


<span data-ttu-id="f5ee2-108">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="f5ee2-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f5ee2-109">属性</span><span class="sxs-lookup"><span data-stu-id="f5ee2-109">Properties</span></span>
|<span data-ttu-id="f5ee2-110">属性</span><span class="sxs-lookup"><span data-stu-id="f5ee2-110">Property</span></span>|<span data-ttu-id="f5ee2-111">类型</span><span class="sxs-lookup"><span data-stu-id="f5ee2-111">Type</span></span>|<span data-ttu-id="f5ee2-112">说明</span><span class="sxs-lookup"><span data-stu-id="f5ee2-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5ee2-113">名</span><span class="sxs-lookup"><span data-stu-id="f5ee2-113">groupName</span></span>|<span data-ttu-id="f5ee2-114">String</span><span class="sxs-lookup"><span data-stu-id="f5ee2-114">String</span></span>|<span data-ttu-id="f5ee2-115">将锁定到此展台配置的 AD 组的名称</span><span class="sxs-lookup"><span data-stu-id="f5ee2-115">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5ee2-116">关系</span><span class="sxs-lookup"><span data-stu-id="f5ee2-116">Relationships</span></span>
<span data-ttu-id="f5ee2-117">无</span><span class="sxs-lookup"><span data-stu-id="f5ee2-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5ee2-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f5ee2-118">JSON Representation</span></span>
<span data-ttu-id="f5ee2-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5ee2-119">Here is a JSON representation of the resource.</span></span>
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



