---
title: userRegistrationFeatureCount 资源类型
description: 注册或能够进行多重身份验证、密码重置Self-Service无密码身份验证的用户数量。
author: danielwood95
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 7c73d9cd17d5bf13eb5f8899e0d1e9dc6e27af67
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132942"
---
# <a name="userregistrationfeaturecount-resource-type"></a><span data-ttu-id="bf58a-103">userRegistrationFeatureCount 资源类型</span><span class="sxs-lookup"><span data-stu-id="bf58a-103">userRegistrationFeatureCount resource type</span></span>

<span data-ttu-id="bf58a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf58a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf58a-105">表示注册或支持多重身份验证、密码重置和无Self-Service身份验证的用户数。</span><span class="sxs-lookup"><span data-stu-id="bf58a-105">Represents the number of users registered or capable for Multi-Factor Authentication, Self-Service Password Reset and Passwordless Authentication.</span></span>

## <a name="properties"></a><span data-ttu-id="bf58a-106">属性</span><span class="sxs-lookup"><span data-stu-id="bf58a-106">Properties</span></span>
|<span data-ttu-id="bf58a-107">属性</span><span class="sxs-lookup"><span data-stu-id="bf58a-107">Property</span></span>|<span data-ttu-id="bf58a-108">类型</span><span class="sxs-lookup"><span data-stu-id="bf58a-108">Type</span></span>|<span data-ttu-id="bf58a-109">说明</span><span class="sxs-lookup"><span data-stu-id="bf58a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf58a-110">功能</span><span class="sxs-lookup"><span data-stu-id="bf58a-110">feature</span></span>|<span data-ttu-id="bf58a-111">authenticationMethodFeature</span><span class="sxs-lookup"><span data-stu-id="bf58a-111">authenticationMethodFeature</span></span>|<span data-ttu-id="bf58a-112">注册或能够进行多重身份验证、密码重置Self-Service无密码身份验证的用户数量。</span><span class="sxs-lookup"><span data-stu-id="bf58a-112">Number of users registered or capable for Multi-Factor Authentication, Self-Service Password Reset and Passwordless Authentication.</span></span> <span data-ttu-id="bf58a-113">可取值为：`ssprRegistered`、`ssprEnabled`、`ssprCapable`、`passwordlessCapable`、`mfaCapable`。</span><span class="sxs-lookup"><span data-stu-id="bf58a-113">Possible values are: `ssprRegistered`, `ssprEnabled`, `ssprCapable`, `passwordlessCapable`, `mfaCapable`.</span></span>|
|<span data-ttu-id="bf58a-114">userCount</span><span class="sxs-lookup"><span data-stu-id="bf58a-114">userCount</span></span>|<span data-ttu-id="bf58a-115">Int64</span><span class="sxs-lookup"><span data-stu-id="bf58a-115">Int64</span></span>|<span data-ttu-id="bf58a-116">用户数。</span><span class="sxs-lookup"><span data-stu-id="bf58a-116">Number of users.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf58a-117">关系</span><span class="sxs-lookup"><span data-stu-id="bf58a-117">Relationships</span></span>
<span data-ttu-id="bf58a-118">无。</span><span class="sxs-lookup"><span data-stu-id="bf58a-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf58a-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf58a-119">JSON representation</span></span>
<span data-ttu-id="bf58a-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf58a-120">The following is a JSON representation of the resource.</span></span>
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
