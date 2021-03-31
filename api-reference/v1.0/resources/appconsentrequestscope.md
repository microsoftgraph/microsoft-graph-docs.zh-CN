---
title: appConsentRequestScope 资源类型
description: 请求访问的动态权限范围的详细信息。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 644ce45997d155a8c3a0bc893af910301e5ba22c
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469553"
---
# <a name="appconsentrequestscope-resource-type"></a><span data-ttu-id="c2265-103">appConsentRequestScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="c2265-103">appConsentRequestScope resource type</span></span>

<span data-ttu-id="c2265-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2265-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c2265-105">**appConsentRequestScope** 详细介绍了请求访问的动态权限范围。</span><span class="sxs-lookup"><span data-stu-id="c2265-105">The **appConsentRequestScope** details the dynamic permission scopes for which access is being requested.</span></span>

## <a name="properties"></a><span data-ttu-id="c2265-106">属性</span><span class="sxs-lookup"><span data-stu-id="c2265-106">Properties</span></span>

|<span data-ttu-id="c2265-107">属性</span><span class="sxs-lookup"><span data-stu-id="c2265-107">Property</span></span>|<span data-ttu-id="c2265-108">类型</span><span class="sxs-lookup"><span data-stu-id="c2265-108">Type</span></span>|<span data-ttu-id="c2265-109">说明</span><span class="sxs-lookup"><span data-stu-id="c2265-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2265-110">displayName</span><span class="sxs-lookup"><span data-stu-id="c2265-110">displayName</span></span>|<span data-ttu-id="c2265-111">String</span><span class="sxs-lookup"><span data-stu-id="c2265-111">String</span></span>|<span data-ttu-id="c2265-112">范围的名称。</span><span class="sxs-lookup"><span data-stu-id="c2265-112">The name of the scope.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2265-113">关系</span><span class="sxs-lookup"><span data-stu-id="c2265-113">Relationships</span></span>

<span data-ttu-id="c2265-114">无。</span><span class="sxs-lookup"><span data-stu-id="c2265-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2265-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2265-115">JSON representation</span></span>

<span data-ttu-id="c2265-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2265-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConsentRequestScope"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.appConsentRequestScope",
  "displayName": "String"
}
```

