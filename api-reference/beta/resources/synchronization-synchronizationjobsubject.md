---
title: synchronizationJobSubject 资源类型
description: 表示将在按需预配时设置的对象。
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f1f7421e00fbf3f974039878e9250f07a2bcbd0b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023833"
---
# <a name="synchronizationjobsubject-resource-type"></a><span data-ttu-id="33104-103">synchronizationJobSubject 资源类型</span><span class="sxs-lookup"><span data-stu-id="33104-103">synchronizationJobSubject resource type</span></span>

<span data-ttu-id="33104-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33104-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="33104-105">表示将在按需预配时设置的对象。</span><span class="sxs-lookup"><span data-stu-id="33104-105">Represents the objects that will be provisioned during on-demand provisioning.</span></span>

## <a name="properties"></a><span data-ttu-id="33104-106">属性</span><span class="sxs-lookup"><span data-stu-id="33104-106">Properties</span></span>
|<span data-ttu-id="33104-107">属性</span><span class="sxs-lookup"><span data-stu-id="33104-107">Property</span></span>|<span data-ttu-id="33104-108">类型</span><span class="sxs-lookup"><span data-stu-id="33104-108">Type</span></span>|<span data-ttu-id="33104-109">说明</span><span class="sxs-lookup"><span data-stu-id="33104-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33104-110">objectId</span><span class="sxs-lookup"><span data-stu-id="33104-110">objectId</span></span>|<span data-ttu-id="33104-111">String</span><span class="sxs-lookup"><span data-stu-id="33104-111">String</span></span>|<span data-ttu-id="33104-112">要应用 synchronizationJob 的对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="33104-112">The identifier of an object to which a synchronizationJob  is to be applied.</span></span>|
|<span data-ttu-id="33104-113">objectTypeName</span><span class="sxs-lookup"><span data-stu-id="33104-113">objectTypeName</span></span>|<span data-ttu-id="33104-114">String</span><span class="sxs-lookup"><span data-stu-id="33104-114">String</span></span>|<span data-ttu-id="33104-115">要应用 synchronizationJob 的对象的类型。</span><span class="sxs-lookup"><span data-stu-id="33104-115">The type of the object to which a synchronizationJob  is to be applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33104-116">关系</span><span class="sxs-lookup"><span data-stu-id="33104-116">Relationships</span></span>
<span data-ttu-id="33104-117">无。</span><span class="sxs-lookup"><span data-stu-id="33104-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="33104-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="33104-118">JSON representation</span></span>
<span data-ttu-id="33104-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33104-119">The following is a JSON representation of the resource.</span></span>
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


