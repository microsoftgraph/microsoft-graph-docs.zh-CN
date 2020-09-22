---
title: mobileContainedApp 资源类型
description: 一个抽象类，表示充当包的 mobileApp 中包含的应用程序。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e60bd8b82847eca69999ea7a05abc0f098d3f5a5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973881"
---
# <a name="mobilecontainedapp-resource-type"></a><span data-ttu-id="f90b1-103">mobileContainedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="f90b1-103">mobileContainedApp resource type</span></span>

<span data-ttu-id="f90b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f90b1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f90b1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f90b1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f90b1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f90b1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f90b1-107">一个抽象类，表示充当包的 mobileApp 中包含的应用程序。</span><span class="sxs-lookup"><span data-stu-id="f90b1-107">An abstract class that represents a contained app in a mobileApp acting as a package.</span></span>

## <a name="methods"></a><span data-ttu-id="f90b1-108">方法</span><span class="sxs-lookup"><span data-stu-id="f90b1-108">Methods</span></span>
|<span data-ttu-id="f90b1-109">方法</span><span class="sxs-lookup"><span data-stu-id="f90b1-109">Method</span></span>|<span data-ttu-id="f90b1-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="f90b1-110">Return Type</span></span>|<span data-ttu-id="f90b1-111">说明</span><span class="sxs-lookup"><span data-stu-id="f90b1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f90b1-112">列出 mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="f90b1-112">List mobileContainedApps</span></span>](../api/intune-apps-mobilecontainedapp-list.md)|<span data-ttu-id="f90b1-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f90b1-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="f90b1-114">列出 [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f90b1-114">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>|
|[<span data-ttu-id="f90b1-115">获取 mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="f90b1-115">Get mobileContainedApp</span></span>](../api/intune-apps-mobilecontainedapp-get.md)|[<span data-ttu-id="f90b1-116">mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="f90b1-116">mobileContainedApp</span></span>](../resources/intune-apps-mobilecontainedapp.md)|<span data-ttu-id="f90b1-117">读取 [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f90b1-117">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f90b1-118">属性</span><span class="sxs-lookup"><span data-stu-id="f90b1-118">Properties</span></span>
|<span data-ttu-id="f90b1-119">属性</span><span class="sxs-lookup"><span data-stu-id="f90b1-119">Property</span></span>|<span data-ttu-id="f90b1-120">类型</span><span class="sxs-lookup"><span data-stu-id="f90b1-120">Type</span></span>|<span data-ttu-id="f90b1-121">说明</span><span class="sxs-lookup"><span data-stu-id="f90b1-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f90b1-122">id</span><span class="sxs-lookup"><span data-stu-id="f90b1-122">id</span></span>|<span data-ttu-id="f90b1-123">String</span><span class="sxs-lookup"><span data-stu-id="f90b1-123">String</span></span>|<span data-ttu-id="f90b1-124">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f90b1-124">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f90b1-125">关系</span><span class="sxs-lookup"><span data-stu-id="f90b1-125">Relationships</span></span>
<span data-ttu-id="f90b1-126">无</span><span class="sxs-lookup"><span data-stu-id="f90b1-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f90b1-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f90b1-127">JSON Representation</span></span>
<span data-ttu-id="f90b1-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f90b1-128">Here is a JSON representation of the resource.</span></span>
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






