---
title: mobileContainedApp 资源类型
description: 一个抽象类, 表示充当包的 mobileApp 中包含的应用程序。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05874102e62e86e5b64fb20c892c2e96c66acfc9
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31795133"
---
# <a name="mobilecontainedapp-resource-type"></a><span data-ttu-id="2f04e-103">mobileContainedApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f04e-103">mobileContainedApp resource type</span></span>

> <span data-ttu-id="2f04e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2f04e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f04e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f04e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f04e-106">一个抽象类, 表示充当包的 mobileApp 中包含的应用程序。</span><span class="sxs-lookup"><span data-stu-id="2f04e-106">An abstract class that represents a contained app in a mobileApp acting as a package.</span></span>

## <a name="methods"></a><span data-ttu-id="2f04e-107">方法</span><span class="sxs-lookup"><span data-stu-id="2f04e-107">Methods</span></span>
|<span data-ttu-id="2f04e-108">方法</span><span class="sxs-lookup"><span data-stu-id="2f04e-108">Method</span></span>|<span data-ttu-id="2f04e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2f04e-109">Return Type</span></span>|<span data-ttu-id="2f04e-110">说明</span><span class="sxs-lookup"><span data-stu-id="2f04e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2f04e-111">列出 mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="2f04e-111">List mobileContainedApps</span></span>](../api/intune-apps-mobilecontainedapp-list.md)|<span data-ttu-id="2f04e-112">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)集合</span><span class="sxs-lookup"><span data-stu-id="2f04e-112">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="2f04e-113">列出[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2f04e-113">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>|
|[<span data-ttu-id="2f04e-114">获取 mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="2f04e-114">Get mobileContainedApp</span></span>](../api/intune-apps-mobilecontainedapp-get.md)|[<span data-ttu-id="2f04e-115">mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="2f04e-115">mobileContainedApp</span></span>](../resources/intune-apps-mobilecontainedapp.md)|<span data-ttu-id="2f04e-116">读取[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2f04e-116">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2f04e-117">属性</span><span class="sxs-lookup"><span data-stu-id="2f04e-117">Properties</span></span>
|<span data-ttu-id="2f04e-118">属性</span><span class="sxs-lookup"><span data-stu-id="2f04e-118">Property</span></span>|<span data-ttu-id="2f04e-119">类型</span><span class="sxs-lookup"><span data-stu-id="2f04e-119">Type</span></span>|<span data-ttu-id="2f04e-120">说明</span><span class="sxs-lookup"><span data-stu-id="2f04e-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f04e-121">id</span><span class="sxs-lookup"><span data-stu-id="2f04e-121">id</span></span>|<span data-ttu-id="2f04e-122">String</span><span class="sxs-lookup"><span data-stu-id="2f04e-122">String</span></span>|<span data-ttu-id="2f04e-123">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2f04e-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f04e-124">关系</span><span class="sxs-lookup"><span data-stu-id="2f04e-124">Relationships</span></span>
<span data-ttu-id="2f04e-125">无</span><span class="sxs-lookup"><span data-stu-id="2f04e-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f04e-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f04e-126">JSON Representation</span></span>
<span data-ttu-id="2f04e-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f04e-127">Here is a JSON representation of the resource.</span></span>
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





