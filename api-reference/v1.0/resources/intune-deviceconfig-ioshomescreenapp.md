---
title: iosHomeScreenApp 资源类型
description: 表示主屏幕上应用的图标
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0c3cf96205d6484c61a6f4ec263566ccb9c2efaa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532512"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="f2f23-103">iosHomeScreenApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2f23-103">iosHomeScreenApp resource type</span></span>

<span data-ttu-id="f2f23-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2f23-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f2f23-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f2f23-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2f23-106">表示主屏幕上应用的图标</span><span class="sxs-lookup"><span data-stu-id="f2f23-106">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="f2f23-107">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="f2f23-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f2f23-108">属性</span><span class="sxs-lookup"><span data-stu-id="f2f23-108">Properties</span></span>
|<span data-ttu-id="f2f23-109">属性</span><span class="sxs-lookup"><span data-stu-id="f2f23-109">Property</span></span>|<span data-ttu-id="f2f23-110">类型</span><span class="sxs-lookup"><span data-stu-id="f2f23-110">Type</span></span>|<span data-ttu-id="f2f23-111">说明</span><span class="sxs-lookup"><span data-stu-id="f2f23-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2f23-112">displayName</span><span class="sxs-lookup"><span data-stu-id="f2f23-112">displayName</span></span>|<span data-ttu-id="f2f23-113">String</span><span class="sxs-lookup"><span data-stu-id="f2f23-113">String</span></span>|<span data-ttu-id="f2f23-114">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="f2f23-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="f2f23-115">bundleID</span><span class="sxs-lookup"><span data-stu-id="f2f23-115">bundleID</span></span>|<span data-ttu-id="f2f23-116">String</span><span class="sxs-lookup"><span data-stu-id="f2f23-116">String</span></span>|<span data-ttu-id="f2f23-117">应用的 BundleID</span><span class="sxs-lookup"><span data-stu-id="f2f23-117">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2f23-118">关系</span><span class="sxs-lookup"><span data-stu-id="f2f23-118">Relationships</span></span>
<span data-ttu-id="f2f23-119">无</span><span class="sxs-lookup"><span data-stu-id="f2f23-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2f23-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2f23-120">JSON Representation</span></span>
<span data-ttu-id="f2f23-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2f23-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```




