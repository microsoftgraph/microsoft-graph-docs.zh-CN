---
title: synchronizationJobSubject 资源类型
description: 表示将在按需预配期间预配的对象。
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: c9e6d83ed7024556954740e89edcc18f7b56ba04
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131996"
---
# <a name="synchronizationjobsubject-resource-type"></a><span data-ttu-id="2dcf5-103">synchronizationJobSubject 资源类型</span><span class="sxs-lookup"><span data-stu-id="2dcf5-103">synchronizationJobSubject resource type</span></span>

<span data-ttu-id="2dcf5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2dcf5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2dcf5-105">表示将在按需预配期间预配的对象。</span><span class="sxs-lookup"><span data-stu-id="2dcf5-105">Represents the objects that will be provisioned during on-demand provisioning.</span></span>

## <a name="properties"></a><span data-ttu-id="2dcf5-106">属性</span><span class="sxs-lookup"><span data-stu-id="2dcf5-106">Properties</span></span>
|<span data-ttu-id="2dcf5-107">属性</span><span class="sxs-lookup"><span data-stu-id="2dcf5-107">Property</span></span>|<span data-ttu-id="2dcf5-108">类型</span><span class="sxs-lookup"><span data-stu-id="2dcf5-108">Type</span></span>|<span data-ttu-id="2dcf5-109">说明</span><span class="sxs-lookup"><span data-stu-id="2dcf5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dcf5-110">objectId</span><span class="sxs-lookup"><span data-stu-id="2dcf5-110">objectId</span></span>|<span data-ttu-id="2dcf5-111">String</span><span class="sxs-lookup"><span data-stu-id="2dcf5-111">String</span></span>|<span data-ttu-id="2dcf5-112">要应用 synchronizationJob 的对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="2dcf5-112">The identifier of an object to which a synchronizationJob  is to be applied.</span></span>|
|<span data-ttu-id="2dcf5-113">objectTypeName</span><span class="sxs-lookup"><span data-stu-id="2dcf5-113">objectTypeName</span></span>|<span data-ttu-id="2dcf5-114">字符串</span><span class="sxs-lookup"><span data-stu-id="2dcf5-114">String</span></span>|<span data-ttu-id="2dcf5-115">要应用 synchronizationJob 的对象的类型。</span><span class="sxs-lookup"><span data-stu-id="2dcf5-115">The type of the object to which a synchronizationJob  is to be applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2dcf5-116">关系</span><span class="sxs-lookup"><span data-stu-id="2dcf5-116">Relationships</span></span>
<span data-ttu-id="2dcf5-117">无。</span><span class="sxs-lookup"><span data-stu-id="2dcf5-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2dcf5-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2dcf5-118">JSON representation</span></span>
<span data-ttu-id="2dcf5-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2dcf5-119">The following is a JSON representation of the resource.</span></span>
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


