---
title: tenantStatusInformation 资源类型
description: 表示托管租户的载入状态信息。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 3e01ac003cda223788e0fc8e6dae01f18667da11
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402268"
---
# <a name="tenantstatusinformation-resource-type"></a><span data-ttu-id="11590-103">tenantStatusInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="11590-103">tenantStatusInformation resource type</span></span>

<span data-ttu-id="11590-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="11590-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11590-105">表示托管租户的载入状态信息。</span><span class="sxs-lookup"><span data-stu-id="11590-105">Represents onboarding status information for a managed tenant.</span></span>

## <a name="properties"></a><span data-ttu-id="11590-106">属性</span><span class="sxs-lookup"><span data-stu-id="11590-106">Properties</span></span>
|<span data-ttu-id="11590-107">属性</span><span class="sxs-lookup"><span data-stu-id="11590-107">Property</span></span>|<span data-ttu-id="11590-108">类型</span><span class="sxs-lookup"><span data-stu-id="11590-108">Type</span></span>|<span data-ttu-id="11590-109">说明</span><span class="sxs-lookup"><span data-stu-id="11590-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11590-110">delegatedPrivilegeStatus</span><span class="sxs-lookup"><span data-stu-id="11590-110">delegatedPrivilegeStatus</span></span>|<span data-ttu-id="11590-111">delegatedPrivilegeStatus</span><span class="sxs-lookup"><span data-stu-id="11590-111">delegatedPrivilegeStatus</span></span>|<span data-ttu-id="11590-112">管理实体与托管租户之间的委派管理员权限关系的状态。</span><span class="sxs-lookup"><span data-stu-id="11590-112">The status of the delegated admin privilege relationship between the managing entity and the managed tenant.</span></span> <span data-ttu-id="11590-113">可取值为：`none`、`delegatedAdminPrivileges`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="11590-113">Possible values are: `none`, `delegatedAdminPrivileges`, `unknownFutureValue`.</span></span> <span data-ttu-id="11590-114">可选。</span><span class="sxs-lookup"><span data-stu-id="11590-114">Optional.</span></span> <span data-ttu-id="11590-115">只读。</span><span class="sxs-lookup"><span data-stu-id="11590-115">Read-only.</span></span>|
|<span data-ttu-id="11590-116">lastDelegatedPrivilegeRefreshDateTime</span><span class="sxs-lookup"><span data-stu-id="11590-116">lastDelegatedPrivilegeRefreshDateTime</span></span>|<span data-ttu-id="11590-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11590-117">DateTimeOffset</span></span>|<span data-ttu-id="11590-118">已更新委派管理员权限状态的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="11590-118">The date and time the delegated admin privileges status was updated.</span></span> <span data-ttu-id="11590-119">可选。</span><span class="sxs-lookup"><span data-stu-id="11590-119">Optional.</span></span> <span data-ttu-id="11590-120">只读。</span><span class="sxs-lookup"><span data-stu-id="11590-120">Read-only.</span></span>|
|<span data-ttu-id="11590-121">offboardedByUserId</span><span class="sxs-lookup"><span data-stu-id="11590-121">offboardedByUserId</span></span>|<span data-ttu-id="11590-122">String</span><span class="sxs-lookup"><span data-stu-id="11590-122">String</span></span>|<span data-ttu-id="11590-123">从托管租户上注销的帐户的标识符。</span><span class="sxs-lookup"><span data-stu-id="11590-123">The identifier for the account that offboarded the managed tenant.</span></span> <span data-ttu-id="11590-124">可选。</span><span class="sxs-lookup"><span data-stu-id="11590-124">Optional.</span></span> <span data-ttu-id="11590-125">只读。</span><span class="sxs-lookup"><span data-stu-id="11590-125">Read-only.</span></span>|
|<span data-ttu-id="11590-126">offboardedDateTime</span><span class="sxs-lookup"><span data-stu-id="11590-126">offboardedDateTime</span></span>|<span data-ttu-id="11590-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11590-127">DateTimeOffset</span></span>|<span data-ttu-id="11590-128">托管租户从外载的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="11590-128">The date and time when the managed tenant was offboarded.</span></span> <span data-ttu-id="11590-129">可选。</span><span class="sxs-lookup"><span data-stu-id="11590-129">Optional.</span></span> <span data-ttu-id="11590-130">只读。</span><span class="sxs-lookup"><span data-stu-id="11590-130">Read-only.</span></span>|
|<span data-ttu-id="11590-131">onboardedByUserId</span><span class="sxs-lookup"><span data-stu-id="11590-131">onboardedByUserId</span></span>|<span data-ttu-id="11590-132">String</span><span class="sxs-lookup"><span data-stu-id="11590-132">String</span></span>|<span data-ttu-id="11590-133">已载入托管租户的帐户的标识符。</span><span class="sxs-lookup"><span data-stu-id="11590-133">The identifier for the account that onboarded the managed tenant.</span></span> <span data-ttu-id="11590-134">可选。</span><span class="sxs-lookup"><span data-stu-id="11590-134">Optional.</span></span> <span data-ttu-id="11590-135">只读。</span><span class="sxs-lookup"><span data-stu-id="11590-135">Read-only.</span></span>|
|<span data-ttu-id="11590-136">onboardedDateTime</span><span class="sxs-lookup"><span data-stu-id="11590-136">onboardedDateTime</span></span>|<span data-ttu-id="11590-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11590-137">DateTimeOffset</span></span>|<span data-ttu-id="11590-138">托管租户载入的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="11590-138">The date and time when the managed tenant was onboarded.</span></span> <span data-ttu-id="11590-139">可选。</span><span class="sxs-lookup"><span data-stu-id="11590-139">Optional.</span></span> <span data-ttu-id="11590-140">只读。</span><span class="sxs-lookup"><span data-stu-id="11590-140">Read-only.</span></span>|
|<span data-ttu-id="11590-141">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="11590-141">onboardingStatus</span></span>|<span data-ttu-id="11590-142">tenantOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="11590-142">tenantOnboardingStatus</span></span>|<span data-ttu-id="11590-143">托管租户的载入状态。</span><span class="sxs-lookup"><span data-stu-id="11590-143">The onboarding status for the managed tenant..</span></span> <span data-ttu-id="11590-144">可取值为：`ineligible`、`inProcess`、`active`、`inactive`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="11590-144">Possible values are: `ineligible`, `inProcess`, `active`, `inactive`, `unknownFutureValue`.</span></span> <span data-ttu-id="11590-145">可选。</span><span class="sxs-lookup"><span data-stu-id="11590-145">Optional.</span></span> <span data-ttu-id="11590-146">只读。</span><span class="sxs-lookup"><span data-stu-id="11590-146">Read-only.</span></span>|
|<span data-ttu-id="11590-147">workloadStatuses</span><span class="sxs-lookup"><span data-stu-id="11590-147">workloadStatuses</span></span>|<span data-ttu-id="11590-148">[microsoft.graph.managedTenants.workloadStatus](../resources/managedtenants-workloadstatus.md) 集合</span><span class="sxs-lookup"><span data-stu-id="11590-148">[microsoft.graph.managedTenants.workloadStatus](../resources/managedtenants-workloadstatus.md) collection</span></span>|<span data-ttu-id="11590-149">托管租户的工作负荷集合。</span><span class="sxs-lookup"><span data-stu-id="11590-149">The collection of workload statues for the managed tenant.</span></span> <span data-ttu-id="11590-150">可选。</span><span class="sxs-lookup"><span data-stu-id="11590-150">Optional.</span></span> <span data-ttu-id="11590-151">只读。</span><span class="sxs-lookup"><span data-stu-id="11590-151">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11590-152">关系</span><span class="sxs-lookup"><span data-stu-id="11590-152">Relationships</span></span>
<span data-ttu-id="11590-153">无。</span><span class="sxs-lookup"><span data-stu-id="11590-153">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="11590-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11590-154">JSON representation</span></span>
<span data-ttu-id="11590-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11590-155">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantStatusInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantStatusInformation",
  "onboardingStatus": "String",
  "onboardedDateTime": "String (timestamp)",
  "onboardedByUserId": "String",
  "offboardedDateTime": "String (timestamp)",
  "offboardedByUserId": "String",
  "delegatedPrivilegeStatus": "String",
  "lastDelegatedPrivilegeRefreshDateTime": "String (timestamp)",
  "workloadStatuses": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadStatus"
    }
  ]
}
```
