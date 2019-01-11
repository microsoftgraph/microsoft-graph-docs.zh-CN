---
title: iosHomeScreenApp 资源类型
description: 表示主屏幕上应用的图标
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bb63950229f88fb9987e75f42abfbe39793864ad
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845694"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="feb14-103">iosHomeScreenApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="feb14-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="feb14-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="feb14-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="feb14-105">表示主屏幕上应用的图标</span><span class="sxs-lookup"><span data-stu-id="feb14-105">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="feb14-106">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="feb14-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="feb14-107">属性</span><span class="sxs-lookup"><span data-stu-id="feb14-107">Properties</span></span>
|<span data-ttu-id="feb14-108">属性</span><span class="sxs-lookup"><span data-stu-id="feb14-108">Property</span></span>|<span data-ttu-id="feb14-109">类型</span><span class="sxs-lookup"><span data-stu-id="feb14-109">Type</span></span>|<span data-ttu-id="feb14-110">说明</span><span class="sxs-lookup"><span data-stu-id="feb14-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="feb14-111">displayName</span><span class="sxs-lookup"><span data-stu-id="feb14-111">displayName</span></span>|<span data-ttu-id="feb14-112">String</span><span class="sxs-lookup"><span data-stu-id="feb14-112">String</span></span>|<span data-ttu-id="feb14-113">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="feb14-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="feb14-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="feb14-114">bundleID</span></span>|<span data-ttu-id="feb14-115">String</span><span class="sxs-lookup"><span data-stu-id="feb14-115">String</span></span>|<span data-ttu-id="feb14-116">应用的 BundleID</span><span class="sxs-lookup"><span data-stu-id="feb14-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="feb14-117">关系</span><span class="sxs-lookup"><span data-stu-id="feb14-117">Relationships</span></span>
<span data-ttu-id="feb14-118">无</span><span class="sxs-lookup"><span data-stu-id="feb14-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="feb14-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="feb14-119">JSON Representation</span></span>
<span data-ttu-id="feb14-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="feb14-120">Here is a JSON representation of the resource.</span></span>
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



