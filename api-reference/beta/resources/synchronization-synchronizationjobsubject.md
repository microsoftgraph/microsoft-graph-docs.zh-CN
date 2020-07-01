---
title: synchronizationJobSubject 资源类型
description: 表示将在按需预配时设置的对象。
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 54f8271d3b11cce55cc3e7042ffcba84a330d798
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007151"
---
# <a name="synchronizationjobsubject-resource-type"></a><span data-ttu-id="a878c-103">synchronizationJobSubject 资源类型</span><span class="sxs-lookup"><span data-stu-id="a878c-103">synchronizationJobSubject resource type</span></span>

<span data-ttu-id="a878c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a878c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a878c-105">表示将在按需预配时设置的对象。</span><span class="sxs-lookup"><span data-stu-id="a878c-105">Represents the objects that will be provisioned during on-demand provisioning.</span></span>

## <a name="properties"></a><span data-ttu-id="a878c-106">属性</span><span class="sxs-lookup"><span data-stu-id="a878c-106">Properties</span></span>
|<span data-ttu-id="a878c-107">属性</span><span class="sxs-lookup"><span data-stu-id="a878c-107">Property</span></span>|<span data-ttu-id="a878c-108">类型</span><span class="sxs-lookup"><span data-stu-id="a878c-108">Type</span></span>|<span data-ttu-id="a878c-109">说明</span><span class="sxs-lookup"><span data-stu-id="a878c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a878c-110">objectId</span><span class="sxs-lookup"><span data-stu-id="a878c-110">objectId</span></span>|<span data-ttu-id="a878c-111">String</span><span class="sxs-lookup"><span data-stu-id="a878c-111">String</span></span>|<span data-ttu-id="a878c-112">要应用 synchronizationJob 的对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="a878c-112">The identifier of an object to which a synchronizationJob  is to be applied.</span></span>|
|<span data-ttu-id="a878c-113">objectTypeName</span><span class="sxs-lookup"><span data-stu-id="a878c-113">objectTypeName</span></span>|<span data-ttu-id="a878c-114">String</span><span class="sxs-lookup"><span data-stu-id="a878c-114">String</span></span>|<span data-ttu-id="a878c-115">要应用 synchronizationJob 的对象的类型。</span><span class="sxs-lookup"><span data-stu-id="a878c-115">The type of the object to which a synchronizationJob  is to be applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a878c-116">关系</span><span class="sxs-lookup"><span data-stu-id="a878c-116">Relationships</span></span>
<span data-ttu-id="a878c-117">无。</span><span class="sxs-lookup"><span data-stu-id="a878c-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a878c-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a878c-118">JSON representation</span></span>
<span data-ttu-id="a878c-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a878c-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationJobSubject"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationJobSubject",
  "objectId": "String",
  "objectTypeName": "String"
}
```
