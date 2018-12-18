---
title: mobileContainedApp 资源类型
description: 表示 mobileApp 充当包中的包含应用程序的抽象类。
author: tfitzmac
ms.openlocfilehash: 314225c46247bd122c825f0f883378513445ce0a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340794"
---
# <a name="mobilecontainedapp-resource-type"></a><span data-ttu-id="2200e-103">mobileContainedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="2200e-103">mobileContainedApp resource type</span></span>

> <span data-ttu-id="2200e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2200e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2200e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2200e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2200e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2200e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2200e-107">表示 mobileApp 充当包中的包含应用程序的抽象类。</span><span class="sxs-lookup"><span data-stu-id="2200e-107">An abstract class that represents a contained app in a mobileApp acting as a package.</span></span>
## <a name="methods"></a><span data-ttu-id="2200e-108">方法</span><span class="sxs-lookup"><span data-stu-id="2200e-108">Methods</span></span>
|<span data-ttu-id="2200e-109">方法</span><span class="sxs-lookup"><span data-stu-id="2200e-109">Method</span></span>|<span data-ttu-id="2200e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="2200e-110">Return Type</span></span>|<span data-ttu-id="2200e-111">说明</span><span class="sxs-lookup"><span data-stu-id="2200e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2200e-112">列表 mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="2200e-112">List mobileContainedApps</span></span>](../api/intune-apps-mobilecontainedapp-list.md)|<span data-ttu-id="2200e-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="2200e-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="2200e-114">列出属性和[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="2200e-114">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>|
|[<span data-ttu-id="2200e-115">获取 mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="2200e-115">Get mobileContainedApp</span></span>](../api/intune-apps-mobilecontainedapp-get.md)|[<span data-ttu-id="2200e-116">mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="2200e-116">mobileContainedApp</span></span>](../resources/intune-apps-mobilecontainedapp.md)|<span data-ttu-id="2200e-117">读取属性和[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="2200e-117">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2200e-118">属性</span><span class="sxs-lookup"><span data-stu-id="2200e-118">Properties</span></span>
|<span data-ttu-id="2200e-119">属性</span><span class="sxs-lookup"><span data-stu-id="2200e-119">Property</span></span>|<span data-ttu-id="2200e-120">类型</span><span class="sxs-lookup"><span data-stu-id="2200e-120">Type</span></span>|<span data-ttu-id="2200e-121">说明</span><span class="sxs-lookup"><span data-stu-id="2200e-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2200e-122">id</span><span class="sxs-lookup"><span data-stu-id="2200e-122">id</span></span>|<span data-ttu-id="2200e-123">String</span><span class="sxs-lookup"><span data-stu-id="2200e-123">String</span></span>|<span data-ttu-id="2200e-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2200e-124">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2200e-125">关系</span><span class="sxs-lookup"><span data-stu-id="2200e-125">Relationships</span></span>
<span data-ttu-id="2200e-126">无</span><span class="sxs-lookup"><span data-stu-id="2200e-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2200e-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2200e-127">JSON Representation</span></span>
<span data-ttu-id="2200e-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2200e-128">Here is a JSON representation of the resource.</span></span>
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





