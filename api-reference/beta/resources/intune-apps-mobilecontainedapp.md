---
title: mobileContainedApp 资源类型
description: 表示 mobileApp 充当包中的包含应用程序的抽象类。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5a9b36193aeda51679018bc534974c3678326a19
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963813"
---
# <a name="mobilecontainedapp-resource-type"></a><span data-ttu-id="913e8-103">mobileContainedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="913e8-103">mobileContainedApp resource type</span></span>

> <span data-ttu-id="913e8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="913e8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="913e8-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="913e8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="913e8-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="913e8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="913e8-107">表示 mobileApp 充当包中的包含应用程序的抽象类。</span><span class="sxs-lookup"><span data-stu-id="913e8-107">An abstract class that represents a contained app in a mobileApp acting as a package.</span></span>
## <a name="methods"></a><span data-ttu-id="913e8-108">方法</span><span class="sxs-lookup"><span data-stu-id="913e8-108">Methods</span></span>
|<span data-ttu-id="913e8-109">方法</span><span class="sxs-lookup"><span data-stu-id="913e8-109">Method</span></span>|<span data-ttu-id="913e8-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="913e8-110">Return Type</span></span>|<span data-ttu-id="913e8-111">说明</span><span class="sxs-lookup"><span data-stu-id="913e8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="913e8-112">列表 mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="913e8-112">List mobileContainedApps</span></span>](../api/intune-apps-mobilecontainedapp-list.md)|<span data-ttu-id="913e8-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="913e8-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="913e8-114">列出属性和[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="913e8-114">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>|
|[<span data-ttu-id="913e8-115">获取 mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="913e8-115">Get mobileContainedApp</span></span>](../api/intune-apps-mobilecontainedapp-get.md)|[<span data-ttu-id="913e8-116">mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="913e8-116">mobileContainedApp</span></span>](../resources/intune-apps-mobilecontainedapp.md)|<span data-ttu-id="913e8-117">读取属性和[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="913e8-117">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="913e8-118">属性</span><span class="sxs-lookup"><span data-stu-id="913e8-118">Properties</span></span>
|<span data-ttu-id="913e8-119">属性</span><span class="sxs-lookup"><span data-stu-id="913e8-119">Property</span></span>|<span data-ttu-id="913e8-120">类型</span><span class="sxs-lookup"><span data-stu-id="913e8-120">Type</span></span>|<span data-ttu-id="913e8-121">说明</span><span class="sxs-lookup"><span data-stu-id="913e8-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="913e8-122">id</span><span class="sxs-lookup"><span data-stu-id="913e8-122">id</span></span>|<span data-ttu-id="913e8-123">String</span><span class="sxs-lookup"><span data-stu-id="913e8-123">String</span></span>|<span data-ttu-id="913e8-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="913e8-124">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="913e8-125">关系</span><span class="sxs-lookup"><span data-stu-id="913e8-125">Relationships</span></span>
<span data-ttu-id="913e8-126">无</span><span class="sxs-lookup"><span data-stu-id="913e8-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="913e8-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="913e8-127">JSON Representation</span></span>
<span data-ttu-id="913e8-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="913e8-128">Here is a JSON representation of the resource.</span></span>
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





