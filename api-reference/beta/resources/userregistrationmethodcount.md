---
title: userRegistrationMethodCount 资源类型
description: 为身份验证方法注册的用户数。
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: b61cb0448c131fc49df43154522e587644d13dc6
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052575"
---
# <a name="userregistrationmethodcount-resource-type"></a><span data-ttu-id="cf8a1-103">userRegistrationMethodCount 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf8a1-103">userRegistrationMethodCount resource type</span></span>

<span data-ttu-id="cf8a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf8a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf8a1-105">为身份验证方法注册的用户数。</span><span class="sxs-lookup"><span data-stu-id="cf8a1-105">Number of users registered for an authentication method.</span></span>

## <a name="properties"></a><span data-ttu-id="cf8a1-106">属性</span><span class="sxs-lookup"><span data-stu-id="cf8a1-106">Properties</span></span>
|<span data-ttu-id="cf8a1-107">属性</span><span class="sxs-lookup"><span data-stu-id="cf8a1-107">Property</span></span>|<span data-ttu-id="cf8a1-108">类型</span><span class="sxs-lookup"><span data-stu-id="cf8a1-108">Type</span></span>|<span data-ttu-id="cf8a1-109">说明</span><span class="sxs-lookup"><span data-stu-id="cf8a1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf8a1-110">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cf8a1-110">authenticationMethod</span></span>|<span data-ttu-id="cf8a1-111">String</span><span class="sxs-lookup"><span data-stu-id="cf8a1-111">String</span></span>|<span data-ttu-id="cf8a1-112">身份验证方法的名称。</span><span class="sxs-lookup"><span data-stu-id="cf8a1-112">Name of authentication method.</span></span>|
|<span data-ttu-id="cf8a1-113">userCount</span><span class="sxs-lookup"><span data-stu-id="cf8a1-113">userCount</span></span>|<span data-ttu-id="cf8a1-114">Int64</span><span class="sxs-lookup"><span data-stu-id="cf8a1-114">Int64</span></span>|<span data-ttu-id="cf8a1-115">注册的用户数。</span><span class="sxs-lookup"><span data-stu-id="cf8a1-115">Number of users registered.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf8a1-116">关系</span><span class="sxs-lookup"><span data-stu-id="cf8a1-116">Relationships</span></span>
<span data-ttu-id="cf8a1-117">无。</span><span class="sxs-lookup"><span data-stu-id="cf8a1-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf8a1-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf8a1-118">JSON representation</span></span>
<span data-ttu-id="cf8a1-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf8a1-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationMethodCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationMethodCount",
  "authenticationMethod": "String",
  "userCount": "Integer"
}
```