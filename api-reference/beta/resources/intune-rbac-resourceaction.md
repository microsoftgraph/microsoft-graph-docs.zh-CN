---
title: resourceAction 资源类型
description: 资源的允许和不允许的操作的集合。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2b8d176b64b6eacc7fbf34a4fe5e15a88da709f2
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48733180"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="b7bc0-103">resourceAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="b7bc0-103">resourceAction resource type</span></span>

<span data-ttu-id="b7bc0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7bc0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7bc0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b7bc0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7bc0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b7bc0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7bc0-107">资源的允许和不允许的操作的集合。</span><span class="sxs-lookup"><span data-stu-id="b7bc0-107">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="b7bc0-108">属性</span><span class="sxs-lookup"><span data-stu-id="b7bc0-108">Properties</span></span>
|<span data-ttu-id="b7bc0-109">属性</span><span class="sxs-lookup"><span data-stu-id="b7bc0-109">Property</span></span>|<span data-ttu-id="b7bc0-110">类型</span><span class="sxs-lookup"><span data-stu-id="b7bc0-110">Type</span></span>|<span data-ttu-id="b7bc0-111">说明</span><span class="sxs-lookup"><span data-stu-id="b7bc0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7bc0-112">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="b7bc0-112">allowedResourceActions</span></span>|<span data-ttu-id="b7bc0-113">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b7bc0-113">String collection</span></span>|<span data-ttu-id="b7bc0-114">允许的操作</span><span class="sxs-lookup"><span data-stu-id="b7bc0-114">Allowed Actions</span></span>|
|<span data-ttu-id="b7bc0-115">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="b7bc0-115">notAllowedResourceActions</span></span>|<span data-ttu-id="b7bc0-116">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b7bc0-116">String collection</span></span>|<span data-ttu-id="b7bc0-117">不允许操作。</span><span class="sxs-lookup"><span data-stu-id="b7bc0-117">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7bc0-118">关系</span><span class="sxs-lookup"><span data-stu-id="b7bc0-118">Relationships</span></span>
<span data-ttu-id="b7bc0-119">无</span><span class="sxs-lookup"><span data-stu-id="b7bc0-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7bc0-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b7bc0-120">JSON Representation</span></span>
<span data-ttu-id="b7bc0-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7bc0-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```





