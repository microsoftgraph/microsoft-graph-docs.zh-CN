---
title: authenticationDetail 资源类型
description: 提供用户登录的身份验证详细信息，如多因素身份验证（MFA）信息和 PTA/PHS 详细信息。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 97375635d86b1be8149035c94d183026a3d49a25
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508085"
---
# <a name="authenticationdetail-resource-type"></a><span data-ttu-id="76c9d-103">authenticationDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="76c9d-103">authenticationDetail resource type</span></span>

<span data-ttu-id="76c9d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="76c9d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76c9d-105">提供用户登录的身份验证详细信息，如多因素身份验证（MFA）信息和 PTA/PHS 详细信息。</span><span class="sxs-lookup"><span data-stu-id="76c9d-105">Provides the authentication details for a user sign-in, such as multi-factor authentication (MFA) information and PTA/PHS details.</span></span>

## <a name="properties"></a><span data-ttu-id="76c9d-106">属性</span><span class="sxs-lookup"><span data-stu-id="76c9d-106">Properties</span></span>

| <span data-ttu-id="76c9d-107">属性</span><span class="sxs-lookup"><span data-stu-id="76c9d-107">Property</span></span>     | <span data-ttu-id="76c9d-108">类型</span><span class="sxs-lookup"><span data-stu-id="76c9d-108">Type</span></span>        | <span data-ttu-id="76c9d-109">说明</span><span class="sxs-lookup"><span data-stu-id="76c9d-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="76c9d-110">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="76c9d-110">authenticationMethod</span></span>|<span data-ttu-id="76c9d-111">String</span><span class="sxs-lookup"><span data-stu-id="76c9d-111">String</span></span>||<span data-ttu-id="76c9d-112">用于执行此身份验证步骤的身份验证方法的类型。</span><span class="sxs-lookup"><span data-stu-id="76c9d-112">The type of authentication method used to perform this step of authentication.</span></span> <span data-ttu-id="76c9d-113">可能的值`Password`： `SMS`、 `Voice`、` Authenticator App`、 `Software OATH token`、 `Satisfied by token`、。</span><span class="sxs-lookup"><span data-stu-id="76c9d-113">Possible values: `Password`, `SMS`, `Voice`,` Authenticator App`, `Software OATH token`, `Satisfied by token`.</span></span>|
|<span data-ttu-id="76c9d-114">authenticationMethodDetail</span><span class="sxs-lookup"><span data-stu-id="76c9d-114">authenticationMethodDetail</span></span>|<span data-ttu-id="76c9d-115">String</span><span class="sxs-lookup"><span data-stu-id="76c9d-115">String</span></span>|<span data-ttu-id="76c9d-116">有关用于执行此身份验证步骤的身份验证方法的详细信息。</span><span class="sxs-lookup"><span data-stu-id="76c9d-116">Details about the authentication method used to perform this authentication step.</span></span> <span data-ttu-id="76c9d-117">例如，电话号码（用于短信和语音）、设备名称（用于验证器应用）和密码源（例如，云、AD FS、PTA、PHS）。</span><span class="sxs-lookup"><span data-stu-id="76c9d-117">For example, phone number (for SMS and voice), device name (for Authenticator app), and password source (e.g. cloud, AD FS, PTA, PHS).</span></span> |
|<span data-ttu-id="76c9d-118">authenticationStepDateTime</span><span class="sxs-lookup"><span data-stu-id="76c9d-118">authenticationStepDateTime</span></span>|<span data-ttu-id="76c9d-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76c9d-119">DateTimeOffset</span></span>|<span data-ttu-id="76c9d-120">表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="76c9d-120">Represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="76c9d-121">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="76c9d-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
|<span data-ttu-id="76c9d-122">authenticationStepRequirement</span><span class="sxs-lookup"><span data-stu-id="76c9d-122">authenticationStepRequirement</span></span>|<span data-ttu-id="76c9d-123">String</span><span class="sxs-lookup"><span data-stu-id="76c9d-123">String</span></span>|<span data-ttu-id="76c9d-124">满足此要求的身份验证步骤。</span><span class="sxs-lookup"><span data-stu-id="76c9d-124">The step of authentication that this satisfied.</span></span> <span data-ttu-id="76c9d-125">例如，主身份验证或多重身份验证。</span><span class="sxs-lookup"><span data-stu-id="76c9d-125">For example, primary authentication, or multi-factor authentication.</span></span>|
|<span data-ttu-id="76c9d-126">authenticationStepResultDetail</span><span class="sxs-lookup"><span data-stu-id="76c9d-126">authenticationStepResultDetail</span></span>|<span data-ttu-id="76c9d-127">String</span><span class="sxs-lookup"><span data-stu-id="76c9d-127">String</span></span>|<span data-ttu-id="76c9d-128">有关步骤成功或失败的原因的详细信息。</span><span class="sxs-lookup"><span data-stu-id="76c9d-128">Details about why the step succeeded or failed.</span></span> <span data-ttu-id="76c9d-129">例如，阻止用户、输入欺诈代码、无电话输入超时、无法连接电话或令牌中的声明。</span><span class="sxs-lookup"><span data-stu-id="76c9d-129">For examples, user is blocked, fraud code entered, no phone input - timed out, phone unreachable, or claim in token.</span></span>|
|<span data-ttu-id="76c9d-130">完成</span><span class="sxs-lookup"><span data-stu-id="76c9d-130">succeeded</span></span>|<span data-ttu-id="76c9d-131">布尔</span><span class="sxs-lookup"><span data-stu-id="76c9d-131">Boolean</span></span>|<span data-ttu-id="76c9d-132">指示身份验证步骤的状态。</span><span class="sxs-lookup"><span data-stu-id="76c9d-132">Indicates the status of the authentication step.</span></span>|<span data-ttu-id="76c9d-133">可能的值`succeeded`： `failed`、。</span><span class="sxs-lookup"><span data-stu-id="76c9d-133">Possible values: `succeeded`, `failed`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="76c9d-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="76c9d-134">JSON representation</span></span>

<span data-ttu-id="76c9d-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76c9d-135">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.authenticationDetail",
  "baseType": null
}-->

```json
{
  "authenticationMethod": "String",
  "authenticationMethodDetail": "String",
  "authenticationStepDateTime": "String (timestamp)",
  "authenticationStepRequirement": "String",
  "authenticationStepResultDetail": "String",
  "succeeded": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "authenticationDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->