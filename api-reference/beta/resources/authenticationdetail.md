---
title: authenticationDetail 资源类型
description: 提供用户登录的身份验证详细信息，例如多重身份验证 (MFA) 和 PTA/PHS 详细信息。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 0f7042b8b2be369c97e19cb038d7cf82fe07e96d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964556"
---
# <a name="authenticationdetail-resource-type"></a><span data-ttu-id="f98e7-103">authenticationDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="f98e7-103">authenticationDetail resource type</span></span>

<span data-ttu-id="f98e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f98e7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f98e7-105">提供用户登录的身份验证详细信息，例如多重身份验证 (MFA) 和 PTA/PHS 详细信息。</span><span class="sxs-lookup"><span data-stu-id="f98e7-105">Provides the authentication details for a user sign-in, such as multi-factor authentication (MFA) information and PTA/PHS details.</span></span>

## <a name="properties"></a><span data-ttu-id="f98e7-106">属性</span><span class="sxs-lookup"><span data-stu-id="f98e7-106">Properties</span></span>

| <span data-ttu-id="f98e7-107">属性</span><span class="sxs-lookup"><span data-stu-id="f98e7-107">Property</span></span>                       | <span data-ttu-id="f98e7-108">类型</span><span class="sxs-lookup"><span data-stu-id="f98e7-108">Type</span></span>           | <span data-ttu-id="f98e7-109">说明</span><span class="sxs-lookup"><span data-stu-id="f98e7-109">Description</span></span>                                                                                                                                                                                                              |
|:-------------------------------|:---------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f98e7-110">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f98e7-110">authenticationMethod</span></span>           | <span data-ttu-id="f98e7-111">String</span><span class="sxs-lookup"><span data-stu-id="f98e7-111">String</span></span>         | <span data-ttu-id="f98e7-112">用于执行此身份验证步骤的身份验证方法的类型。</span><span class="sxs-lookup"><span data-stu-id="f98e7-112">The type of authentication method used to perform this step of authentication.</span></span> <span data-ttu-id="f98e7-113">可能的值 `Password` `SMS` `Voice` ：、、、、、、。 `Authenticator App` `Software OATH token` `Satisfied by token` `Previously satisfied`</span><span class="sxs-lookup"><span data-stu-id="f98e7-113">Possible values: `Password`, `SMS`, `Voice`, `Authenticator App`, `Software OATH token`, `Satisfied by token`, `Previously satisfied`.</span></span>                            |
| <span data-ttu-id="f98e7-114">authenticationMethodDetail</span><span class="sxs-lookup"><span data-stu-id="f98e7-114">authenticationMethodDetail</span></span>     | <span data-ttu-id="f98e7-115">String</span><span class="sxs-lookup"><span data-stu-id="f98e7-115">String</span></span>         | <span data-ttu-id="f98e7-116">有关用于执行此身份验证步骤的身份验证方法的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f98e7-116">Details about the authentication method used to perform this authentication step.</span></span> <span data-ttu-id="f98e7-117">例如，短信 (语音) 的电话号码、用于 Authenticator) 的设备名称 (以及密码源 (例如云、AD FS、PTA、PHS) 。</span><span class="sxs-lookup"><span data-stu-id="f98e7-117">For example, phone number (for SMS and voice), device name (for Authenticator app), and password source (e.g. cloud, AD FS, PTA, PHS).</span></span> |
| <span data-ttu-id="f98e7-118">authenticationStepDateTime</span><span class="sxs-lookup"><span data-stu-id="f98e7-118">authenticationStepDateTime</span></span>     | <span data-ttu-id="f98e7-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f98e7-119">DateTimeOffset</span></span> | <span data-ttu-id="f98e7-120">表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="f98e7-120">Represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f98e7-121">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="f98e7-121">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>                                           |
| <span data-ttu-id="f98e7-122">authenticationStepRequirement</span><span class="sxs-lookup"><span data-stu-id="f98e7-122">authenticationStepRequirement</span></span>  | <span data-ttu-id="f98e7-123">String</span><span class="sxs-lookup"><span data-stu-id="f98e7-123">String</span></span>         | <span data-ttu-id="f98e7-124">符合此要求的身份验证步骤。</span><span class="sxs-lookup"><span data-stu-id="f98e7-124">The step of authentication that this satisfied.</span></span> <span data-ttu-id="f98e7-125">例如，主身份验证或多重身份验证。</span><span class="sxs-lookup"><span data-stu-id="f98e7-125">For example, primary authentication, or multi-factor authentication.</span></span>                                                                                                     |
| <span data-ttu-id="f98e7-126">authenticationStepResultDetail</span><span class="sxs-lookup"><span data-stu-id="f98e7-126">authenticationStepResultDetail</span></span> | <span data-ttu-id="f98e7-127">String</span><span class="sxs-lookup"><span data-stu-id="f98e7-127">String</span></span>         | <span data-ttu-id="f98e7-128">有关步骤成功或失败的原因的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f98e7-128">Details about why the step succeeded or failed.</span></span> <span data-ttu-id="f98e7-129">例如，用户被阻止、输入欺诈代码、没有电话输入 - 已注销、电话无法访问或令牌中声明。</span><span class="sxs-lookup"><span data-stu-id="f98e7-129">For examples, user is blocked, fraud code entered, no phone input - timed out, phone unreachable, or claim in token.</span></span>                                                     |
| <span data-ttu-id="f98e7-130">succeeded</span><span class="sxs-lookup"><span data-stu-id="f98e7-130">succeeded</span></span>                      | <span data-ttu-id="f98e7-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="f98e7-131">Boolean</span></span>        | <span data-ttu-id="f98e7-132">指示身份验证步骤的状态。</span><span class="sxs-lookup"><span data-stu-id="f98e7-132">Indicates the status of the authentication step.</span></span> <span data-ttu-id="f98e7-133">可能的值 `succeeded` `failed` ：、。</span><span class="sxs-lookup"><span data-stu-id="f98e7-133">Possible values: `succeeded`, `failed`.</span></span>                                                                                                                                 |

## <a name="json-representation"></a><span data-ttu-id="f98e7-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f98e7-134">JSON representation</span></span>

<span data-ttu-id="f98e7-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f98e7-135">The following is a JSON representation of the resource.</span></span>

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

