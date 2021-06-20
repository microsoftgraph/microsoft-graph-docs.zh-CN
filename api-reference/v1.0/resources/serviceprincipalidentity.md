---
title: servicePrincipalIdentity 资源类型
description: 为服务主体标识创建模型。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 231a0d9dc811569de23412d6ad76a2ba35f6c58b
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031087"
---
# <a name="serviceprincipalidentity-resource-type"></a><span data-ttu-id="85055-103">servicePrincipalIdentity 资源类型</span><span class="sxs-lookup"><span data-stu-id="85055-103">servicePrincipalIdentity resource type</span></span>

<span data-ttu-id="85055-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85055-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="85055-105">为服务主体标识创建模型。</span><span class="sxs-lookup"><span data-stu-id="85055-105">Models a service principal identity.</span></span>

<span data-ttu-id="85055-106">继承自 [标识](../resources/identity.md)。</span><span class="sxs-lookup"><span data-stu-id="85055-106">Inherits from [identity](../resources/identity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="85055-107">属性</span><span class="sxs-lookup"><span data-stu-id="85055-107">Properties</span></span>
|<span data-ttu-id="85055-108">属性</span><span class="sxs-lookup"><span data-stu-id="85055-108">Property</span></span>|<span data-ttu-id="85055-109">类型</span><span class="sxs-lookup"><span data-stu-id="85055-109">Type</span></span>|<span data-ttu-id="85055-110">说明</span><span class="sxs-lookup"><span data-stu-id="85055-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85055-111">appId</span><span class="sxs-lookup"><span data-stu-id="85055-111">appId</span></span>|<span data-ttu-id="85055-112">String</span><span class="sxs-lookup"><span data-stu-id="85055-112">String</span></span>|<span data-ttu-id="85055-113">服务主体的应用程序标识符。</span><span class="sxs-lookup"><span data-stu-id="85055-113">The application identifier of the service principal.</span></span>|
|<span data-ttu-id="85055-114">displayName</span><span class="sxs-lookup"><span data-stu-id="85055-114">displayName</span></span>|<span data-ttu-id="85055-115">String</span><span class="sxs-lookup"><span data-stu-id="85055-115">String</span></span>|<span data-ttu-id="85055-116">服务显示名称标识的组。</span><span class="sxs-lookup"><span data-stu-id="85055-116">The display name of the service principal identity.</span></span> <span data-ttu-id="85055-117">继承自 [标识](../resources/identity.md)</span><span class="sxs-lookup"><span data-stu-id="85055-117">Inherited from [identity](../resources/identity.md)</span></span>|
|<span data-ttu-id="85055-118">id</span><span class="sxs-lookup"><span data-stu-id="85055-118">id</span></span>|<span data-ttu-id="85055-119">String</span><span class="sxs-lookup"><span data-stu-id="85055-119">String</span></span>|<span data-ttu-id="85055-120">服务主体标识的标识符。</span><span class="sxs-lookup"><span data-stu-id="85055-120">The identifier of the service principal identity.</span></span> <span data-ttu-id="85055-121">继承自 [标识](../resources/identity.md)</span><span class="sxs-lookup"><span data-stu-id="85055-121">Inherited from [identity](../resources/identity.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="85055-122">关系</span><span class="sxs-lookup"><span data-stu-id="85055-122">Relationships</span></span>
<span data-ttu-id="85055-123">无。</span><span class="sxs-lookup"><span data-stu-id="85055-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="85055-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85055-124">JSON representation</span></span>
<span data-ttu-id="85055-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85055-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.servicePrincipalIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.servicePrincipalIdentity",
  "id": "String (identifier)",
  "displayName": "String",
  "appId": "String"
}
```
