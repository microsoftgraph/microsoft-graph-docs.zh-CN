---
title: excludeTarget 资源类型
description: 表示从策略中排除的用户或用户组。
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9d2786a6107e524fe00430658542dea374cae275
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682884"
---
# <a name="excludetarget-resource-type"></a><span data-ttu-id="7ae1e-103">excludeTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ae1e-103">excludeTarget resource type</span></span>

<span data-ttu-id="7ae1e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ae1e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ae1e-105">表示从策略中排除的用户或用户组。</span><span class="sxs-lookup"><span data-stu-id="7ae1e-105">Represents the users or groups of users that are excluded from a policy.</span></span>

## <a name="properties"></a><span data-ttu-id="7ae1e-106">属性</span><span class="sxs-lookup"><span data-stu-id="7ae1e-106">Properties</span></span>
|<span data-ttu-id="7ae1e-107">属性</span><span class="sxs-lookup"><span data-stu-id="7ae1e-107">Property</span></span>|<span data-ttu-id="7ae1e-108">类型</span><span class="sxs-lookup"><span data-stu-id="7ae1e-108">Type</span></span>|<span data-ttu-id="7ae1e-109">说明</span><span class="sxs-lookup"><span data-stu-id="7ae1e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ae1e-110">id</span><span class="sxs-lookup"><span data-stu-id="7ae1e-110">id</span></span>|<span data-ttu-id="7ae1e-111">String</span><span class="sxs-lookup"><span data-stu-id="7ae1e-111">String</span></span>|<span data-ttu-id="7ae1e-112">Azure AD 用户或组的对象标识符。</span><span class="sxs-lookup"><span data-stu-id="7ae1e-112">The object identifier of an Azure AD user or group.</span></span>|
|<span data-ttu-id="7ae1e-113">targetType</span><span class="sxs-lookup"><span data-stu-id="7ae1e-113">targetType</span></span>|<span data-ttu-id="7ae1e-114">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="7ae1e-114">authenticationMethodTargetType</span></span>|<span data-ttu-id="7ae1e-115">身份验证方法目标的类型。</span><span class="sxs-lookup"><span data-stu-id="7ae1e-115">The type of the authentication method target.</span></span> <span data-ttu-id="7ae1e-116">可取值为：`user`、`group`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="7ae1e-116">Possible values are: `user`, `group`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ae1e-117">关系</span><span class="sxs-lookup"><span data-stu-id="7ae1e-117">Relationships</span></span>
<span data-ttu-id="7ae1e-118">无。</span><span class="sxs-lookup"><span data-stu-id="7ae1e-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ae1e-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ae1e-119">JSON representation</span></span>
<span data-ttu-id="7ae1e-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ae1e-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.excludeTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.excludeTarget",
  "id": "String (identifier)",
  "targetType": "String"
}
```
