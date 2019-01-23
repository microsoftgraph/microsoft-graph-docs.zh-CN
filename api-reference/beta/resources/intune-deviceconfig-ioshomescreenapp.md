---
title: iosHomeScreenApp 资源类型
description: 表示主屏幕上应用的图标
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dcc90e774f8d032d46968fc4f751923bcc52e559
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412322"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="a8b75-103">iosHomeScreenApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="a8b75-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="a8b75-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a8b75-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a8b75-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a8b75-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8b75-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a8b75-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8b75-107">表示主屏幕上应用的图标</span><span class="sxs-lookup"><span data-stu-id="a8b75-107">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="a8b75-108">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="a8b75-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a8b75-109">属性</span><span class="sxs-lookup"><span data-stu-id="a8b75-109">Properties</span></span>
|<span data-ttu-id="a8b75-110">属性</span><span class="sxs-lookup"><span data-stu-id="a8b75-110">Property</span></span>|<span data-ttu-id="a8b75-111">类型</span><span class="sxs-lookup"><span data-stu-id="a8b75-111">Type</span></span>|<span data-ttu-id="a8b75-112">说明</span><span class="sxs-lookup"><span data-stu-id="a8b75-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8b75-113">displayName</span><span class="sxs-lookup"><span data-stu-id="a8b75-113">displayName</span></span>|<span data-ttu-id="a8b75-114">String</span><span class="sxs-lookup"><span data-stu-id="a8b75-114">String</span></span>|<span data-ttu-id="a8b75-115">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="a8b75-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="a8b75-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="a8b75-116">bundleID</span></span>|<span data-ttu-id="a8b75-117">String</span><span class="sxs-lookup"><span data-stu-id="a8b75-117">String</span></span>|<span data-ttu-id="a8b75-118">应用的 BundleID</span><span class="sxs-lookup"><span data-stu-id="a8b75-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8b75-119">关系</span><span class="sxs-lookup"><span data-stu-id="a8b75-119">Relationships</span></span>
<span data-ttu-id="a8b75-120">无</span><span class="sxs-lookup"><span data-stu-id="a8b75-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8b75-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a8b75-121">JSON Representation</span></span>
<span data-ttu-id="a8b75-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8b75-122">Here is a JSON representation of the resource.</span></span>
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




