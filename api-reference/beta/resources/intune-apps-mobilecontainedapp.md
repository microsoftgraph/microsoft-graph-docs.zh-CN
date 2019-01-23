---
title: mobileContainedApp 资源类型
description: 表示 mobileApp 充当包中的包含应用程序的抽象类。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c5d4ed392d681d97478cb1baf5ff6f854cb74011
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425664"
---
# <a name="mobilecontainedapp-resource-type"></a><span data-ttu-id="9ec75-103">mobileContainedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="9ec75-103">mobileContainedApp resource type</span></span>

> <span data-ttu-id="9ec75-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="9ec75-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9ec75-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9ec75-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ec75-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ec75-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ec75-107">表示 mobileApp 充当包中的包含应用程序的抽象类。</span><span class="sxs-lookup"><span data-stu-id="9ec75-107">An abstract class that represents a contained app in a mobileApp acting as a package.</span></span>

## <a name="methods"></a><span data-ttu-id="9ec75-108">方法</span><span class="sxs-lookup"><span data-stu-id="9ec75-108">Methods</span></span>
|<span data-ttu-id="9ec75-109">方法</span><span class="sxs-lookup"><span data-stu-id="9ec75-109">Method</span></span>|<span data-ttu-id="9ec75-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9ec75-110">Return Type</span></span>|<span data-ttu-id="9ec75-111">说明</span><span class="sxs-lookup"><span data-stu-id="9ec75-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9ec75-112">列表 mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="9ec75-112">List mobileContainedApps</span></span>](../api/intune-apps-mobilecontainedapp-list.md)|<span data-ttu-id="9ec75-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="9ec75-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="9ec75-114">列出属性和[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="9ec75-114">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>|
|[<span data-ttu-id="9ec75-115">获取 mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="9ec75-115">Get mobileContainedApp</span></span>](../api/intune-apps-mobilecontainedapp-get.md)|[<span data-ttu-id="9ec75-116">mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="9ec75-116">mobileContainedApp</span></span>](../resources/intune-apps-mobilecontainedapp.md)|<span data-ttu-id="9ec75-117">读取属性和[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="9ec75-117">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ec75-118">属性</span><span class="sxs-lookup"><span data-stu-id="9ec75-118">Properties</span></span>
|<span data-ttu-id="9ec75-119">属性</span><span class="sxs-lookup"><span data-stu-id="9ec75-119">Property</span></span>|<span data-ttu-id="9ec75-120">类型</span><span class="sxs-lookup"><span data-stu-id="9ec75-120">Type</span></span>|<span data-ttu-id="9ec75-121">说明</span><span class="sxs-lookup"><span data-stu-id="9ec75-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ec75-122">id</span><span class="sxs-lookup"><span data-stu-id="9ec75-122">id</span></span>|<span data-ttu-id="9ec75-123">String</span><span class="sxs-lookup"><span data-stu-id="9ec75-123">String</span></span>|<span data-ttu-id="9ec75-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9ec75-124">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ec75-125">关系</span><span class="sxs-lookup"><span data-stu-id="9ec75-125">Relationships</span></span>
<span data-ttu-id="9ec75-126">无</span><span class="sxs-lookup"><span data-stu-id="9ec75-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ec75-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9ec75-127">JSON Representation</span></span>
<span data-ttu-id="9ec75-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ec75-128">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileContainedApp",
  "id": "String (identifier)"
}
```




