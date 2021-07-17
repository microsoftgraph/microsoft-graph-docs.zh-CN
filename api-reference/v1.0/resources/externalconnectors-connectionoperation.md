---
title: connectionOperation 资源类型
description: 描述创建连接架构的异步请求Microsoft 搜索状态。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: f81300c0fd2f895daccb816c86cdd7151c803b2d
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467276"
---
# <a name="connectionoperation-resource-type"></a><span data-ttu-id="30175-103">connectionOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="30175-103">connectionOperation resource type</span></span>

<span data-ttu-id="30175-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="30175-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="30175-105">描述创建连接架构的异步Microsoft 搜索[状态](externalconnectors-schema.md)。</span><span class="sxs-lookup"><span data-stu-id="30175-105">Describes status of an asynchronous request to create a Microsoft Search connection [schema](externalconnectors-schema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="30175-106">方法</span><span class="sxs-lookup"><span data-stu-id="30175-106">Methods</span></span>
|<span data-ttu-id="30175-107">方法</span><span class="sxs-lookup"><span data-stu-id="30175-107">Method</span></span>|<span data-ttu-id="30175-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="30175-108">Return type</span></span>|<span data-ttu-id="30175-109">说明</span><span class="sxs-lookup"><span data-stu-id="30175-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="30175-110">获取 connectionOperation</span><span class="sxs-lookup"><span data-stu-id="30175-110">Get connectionOperation</span></span>](../api/externalconnectors-connectionoperation-get.md)|[<span data-ttu-id="30175-111">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="30175-111">connectionOperation</span></span>](../resources/externalconnectors-connectionoperation.md)|<span data-ttu-id="30175-112">读取 [connectionOperation](../resources/externalconnectors-connectionoperation.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="30175-112">Read the properties and relationships of a [connectionOperation](../resources/externalconnectors-connectionoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="30175-113">属性</span><span class="sxs-lookup"><span data-stu-id="30175-113">Properties</span></span>
|<span data-ttu-id="30175-114">属性</span><span class="sxs-lookup"><span data-stu-id="30175-114">Property</span></span>|<span data-ttu-id="30175-115">类型</span><span class="sxs-lookup"><span data-stu-id="30175-115">Type</span></span>|<span data-ttu-id="30175-116">说明</span><span class="sxs-lookup"><span data-stu-id="30175-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30175-117">error</span><span class="sxs-lookup"><span data-stu-id="30175-117">error</span></span>|<span data-ttu-id="30175-118">publicError</span><span class="sxs-lookup"><span data-stu-id="30175-118">publicError</span></span>| <span data-ttu-id="30175-119">如果 `status` 为 `failed` ，则提供有关导致失败的错误的详细信息。</span><span class="sxs-lookup"><span data-stu-id="30175-119">If `status` is `failed`, provides more information about the error that caused the failure.</span></span>|
|<span data-ttu-id="30175-120">id</span><span class="sxs-lookup"><span data-stu-id="30175-120">id</span></span>|<span data-ttu-id="30175-121">String</span><span class="sxs-lookup"><span data-stu-id="30175-121">String</span></span>| <span data-ttu-id="30175-122">connectionOperation 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="30175-122">Unique identifier for the connectionOperation.</span></span> <span data-ttu-id="30175-123">只读。</span><span class="sxs-lookup"><span data-stu-id="30175-123">Read-only.</span></span> |
|<span data-ttu-id="30175-124">状态</span><span class="sxs-lookup"><span data-stu-id="30175-124">status</span></span>|<span data-ttu-id="30175-125">microsoft.graph.externalConnectors.connectionOperationStatus</span><span class="sxs-lookup"><span data-stu-id="30175-125">microsoft.graph.externalConnectors.connectionOperationStatus</span></span>| <span data-ttu-id="30175-126">指示异步操作的状态。</span><span class="sxs-lookup"><span data-stu-id="30175-126">Indicates the status of the asynchronous operation.</span></span> <span data-ttu-id="30175-127">可取值为：`unspecified`、`inprogress`、`completed`、`failed`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="30175-127">Possible values are: `unspecified`, `inprogress`, `completed`, `failed`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="30175-128">关系</span><span class="sxs-lookup"><span data-stu-id="30175-128">Relationships</span></span>
<span data-ttu-id="30175-129">无。</span><span class="sxs-lookup"><span data-stu-id="30175-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="30175-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="30175-130">JSON representation</span></span>
<span data-ttu-id="30175-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="30175-131">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.connectionOperation",
  "openType": false
}
-->
``` json
{
  "id": "String (identifier)",
  "status": "String"
}
```

