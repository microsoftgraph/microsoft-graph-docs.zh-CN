---
title: userRegistrationFeatureCount 资源类型
description: 注册或能够进行多重身份验证、密码重置Self-Service无密码身份验证的用户数量。
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 0a0ad3758a74e057fa5539d3d913dd1735c88854
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052570"
---
# <a name="userregistrationfeaturecount-resource-type"></a><span data-ttu-id="26074-103">userRegistrationFeatureCount 资源类型</span><span class="sxs-lookup"><span data-stu-id="26074-103">userRegistrationFeatureCount resource type</span></span>

<span data-ttu-id="26074-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="26074-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26074-105">表示注册或支持多重身份验证、密码重置和无Self-Service身份验证的用户数。</span><span class="sxs-lookup"><span data-stu-id="26074-105">Represents the number of users registered or capable for Multi-Factor Authentication, Self-Service Password Reset and Passwordless Authentication.</span></span>

## <a name="properties"></a><span data-ttu-id="26074-106">属性</span><span class="sxs-lookup"><span data-stu-id="26074-106">Properties</span></span>
|<span data-ttu-id="26074-107">属性</span><span class="sxs-lookup"><span data-stu-id="26074-107">Property</span></span>|<span data-ttu-id="26074-108">类型</span><span class="sxs-lookup"><span data-stu-id="26074-108">Type</span></span>|<span data-ttu-id="26074-109">说明</span><span class="sxs-lookup"><span data-stu-id="26074-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26074-110">功能</span><span class="sxs-lookup"><span data-stu-id="26074-110">feature</span></span>|<span data-ttu-id="26074-111">authenticationMethodFeature</span><span class="sxs-lookup"><span data-stu-id="26074-111">authenticationMethodFeature</span></span>|<span data-ttu-id="26074-112">已注册或能够进行多重身份验证、密码重置Self-Service无密码身份验证的用户数。</span><span class="sxs-lookup"><span data-stu-id="26074-112">Number of users registered or capable for Multi-Factor Authentication, Self-Service Password Reset and Passwordless Authentication.</span></span> <span data-ttu-id="26074-113">可取值为：`ssprRegistered`、`ssprEnabled`、`ssprCapable`、`passwordlessCapable`、`mfaCapable`。</span><span class="sxs-lookup"><span data-stu-id="26074-113">Possible values are: `ssprRegistered`, `ssprEnabled`, `ssprCapable`, `passwordlessCapable`, `mfaCapable`.</span></span>|
|<span data-ttu-id="26074-114">userCount</span><span class="sxs-lookup"><span data-stu-id="26074-114">userCount</span></span>|<span data-ttu-id="26074-115">Int64</span><span class="sxs-lookup"><span data-stu-id="26074-115">Int64</span></span>|<span data-ttu-id="26074-116">用户数。</span><span class="sxs-lookup"><span data-stu-id="26074-116">Number of users.</span></span>|

## <a name="relationships"></a><span data-ttu-id="26074-117">关系</span><span class="sxs-lookup"><span data-stu-id="26074-117">Relationships</span></span>
<span data-ttu-id="26074-118">无。</span><span class="sxs-lookup"><span data-stu-id="26074-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="26074-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="26074-119">JSON representation</span></span>
<span data-ttu-id="26074-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="26074-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationFeatureCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationFeatureCount",
  "feature": "String",
  "userCount": "Integer"
}
```
