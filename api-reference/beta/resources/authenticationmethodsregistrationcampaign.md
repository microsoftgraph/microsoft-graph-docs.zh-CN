---
title: authenticationMethodsRegistrationCampaign 资源类型
description: 表示用于运行市场活动以推送用户设置目标身份验证方法的设置。
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: be989bc86e5e708a89cd33c700e57edce42d9e50
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682879"
---
# <a name="authenticationmethodsregistrationcampaign-resource-type"></a><span data-ttu-id="673af-103">authenticationMethodsRegistrationCampaign 资源类型</span><span class="sxs-lookup"><span data-stu-id="673af-103">authenticationMethodsRegistrationCampaign resource type</span></span>

<span data-ttu-id="673af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="673af-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="673af-105">表示用于运行市场活动以推送用户设置目标身份验证方法的设置。</span><span class="sxs-lookup"><span data-stu-id="673af-105">Represents the settings used to run campaigns to push users to set up targeted authentication methods.</span></span> <span data-ttu-id="673af-106">用户成功完成 MFA 质询后，系统会提示他们设置身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="673af-106">Users are prompted to set up the authentication method after they successfully complete a MFA challenge.</span></span> <span data-ttu-id="673af-107">仅适用于 MFA Microsoft Authenticator应用。</span><span class="sxs-lookup"><span data-stu-id="673af-107">Only available for the Microsoft Authenticator app for MFA.</span></span>

## <a name="properties"></a><span data-ttu-id="673af-108">属性</span><span class="sxs-lookup"><span data-stu-id="673af-108">Properties</span></span>
|<span data-ttu-id="673af-109">属性</span><span class="sxs-lookup"><span data-stu-id="673af-109">Property</span></span>|<span data-ttu-id="673af-110">类型</span><span class="sxs-lookup"><span data-stu-id="673af-110">Type</span></span>|<span data-ttu-id="673af-111">说明</span><span class="sxs-lookup"><span data-stu-id="673af-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="673af-112">excludeTargets</span><span class="sxs-lookup"><span data-stu-id="673af-112">excludeTargets</span></span>|<span data-ttu-id="673af-113">[excludeTarget](../resources/excludetarget.md) 集合</span><span class="sxs-lookup"><span data-stu-id="673af-113">[excludeTarget](../resources/excludetarget.md) collection</span></span>|<span data-ttu-id="673af-114">系统提示他们设置身份验证方法时排除的用户和用户组。</span><span class="sxs-lookup"><span data-stu-id="673af-114">Users and groups of users that are excluded from being prompted to set up the authentication method.</span></span>|
|<span data-ttu-id="673af-115">includeTargets</span><span class="sxs-lookup"><span data-stu-id="673af-115">includeTargets</span></span>|<span data-ttu-id="673af-116">[authenticationMethodsRegistrationCampaignIncludeTarget](../resources/authenticationmethodsregistrationcampaignincludetarget.md) 集合</span><span class="sxs-lookup"><span data-stu-id="673af-116">[authenticationMethodsRegistrationCampaignIncludeTarget](../resources/authenticationmethodsregistrationcampaignincludetarget.md) collection</span></span>|<span data-ttu-id="673af-117">提示设置身份验证方法的用户和用户组。</span><span class="sxs-lookup"><span data-stu-id="673af-117">Users and groups of users that are prompted to set up the authentication method.</span></span>|
|<span data-ttu-id="673af-118">snoozeDurationInDays</span><span class="sxs-lookup"><span data-stu-id="673af-118">snoozeDurationInDays</span></span>|<span data-ttu-id="673af-119">Int32</span><span class="sxs-lookup"><span data-stu-id="673af-119">Int32</span></span>|<span data-ttu-id="673af-120">指定用户在选择"Not now"并暂停提示时再次看到提示的天数。</span><span class="sxs-lookup"><span data-stu-id="673af-120">Specifies the number of days that the user sees a prompt again if they select "Not now" and snoozes the prompt.</span></span> <span data-ttu-id="673af-121">最少 0 天。</span><span class="sxs-lookup"><span data-stu-id="673af-121">Minimum 0 days.</span></span> <span data-ttu-id="673af-122">最大值：14 天。</span><span class="sxs-lookup"><span data-stu-id="673af-122">Maximum: 14 days.</span></span> <span data-ttu-id="673af-123">如果值为"0"- 每次尝试 MFA 时都会提示用户。</span><span class="sxs-lookup"><span data-stu-id="673af-123">If the value is “0” – The user is prompted during every MFA attempt.</span></span>|
|<span data-ttu-id="673af-124">state</span><span class="sxs-lookup"><span data-stu-id="673af-124">state</span></span>|<span data-ttu-id="673af-125">advancedConfigState</span><span class="sxs-lookup"><span data-stu-id="673af-125">advancedConfigState</span></span>|<span data-ttu-id="673af-126">启用或禁用该功能。</span><span class="sxs-lookup"><span data-stu-id="673af-126">Enable or disable the feature.</span></span> <span data-ttu-id="673af-127">可取值为：`default`、`enabled`、`disabled`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="673af-127">Possible values are: `default`, `enabled`, `disabled`, `unknownFutureValue`.</span></span> <span data-ttu-id="673af-128">当配置尚未明确设置并使用 Azure AD 的默认行为进行设置时 `default` ，将使用该值。</span><span class="sxs-lookup"><span data-stu-id="673af-128">The `default` value is used when the configuration hasn't been explicitly set and uses the default behavior of Azure AD for the setting.</span></span> <span data-ttu-id="673af-129">默认值为 `disabled`。</span><span class="sxs-lookup"><span data-stu-id="673af-129">The default value is `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="673af-130">关系</span><span class="sxs-lookup"><span data-stu-id="673af-130">Relationships</span></span>
<span data-ttu-id="673af-131">无。</span><span class="sxs-lookup"><span data-stu-id="673af-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="673af-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="673af-132">JSON representation</span></span>
<span data-ttu-id="673af-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="673af-133">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaign"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsRegistrationCampaign",
  "excludeTargets": [
    {
      "@odata.type": "microsoft.graph.excludeTarget"
    }
  ],
  "includeTargets": [
    {
      "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaignIncludeTarget"
    }
  ],
  "snoozeDurationInDays": "Integer",
  "state": "String"
}
```
