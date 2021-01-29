---
title: userRegistrationFeatureSummary 资源类型
description: 能够进行多重身份验证、密码Self-Service和无密码身份验证的用户摘要。
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 3dc3b48e6883b8c953db5d7b826243989109f2d9
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052571"
---
# <a name="userregistrationfeaturesummary-resource-type"></a><span data-ttu-id="7d5e3-103">userRegistrationFeatureSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d5e3-103">userRegistrationFeatureSummary resource type</span></span>

<span data-ttu-id="7d5e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d5e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7d5e3-105">表示组织中有多少用户能够进行多重身份验证、自助服务密码重置和无密码身份验证的当前状态。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-105">Represents the current state of how many users in your organization are capable of multi-factor authentication, self-service password reset and passwordless authentication.</span></span>

## <a name="methods"></a><span data-ttu-id="7d5e3-106">方法</span><span class="sxs-lookup"><span data-stu-id="7d5e3-106">Methods</span></span>

| <span data-ttu-id="7d5e3-107">方法</span><span class="sxs-lookup"><span data-stu-id="7d5e3-107">Method</span></span>       | <span data-ttu-id="7d5e3-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="7d5e3-108">Return Type</span></span> | <span data-ttu-id="7d5e3-109">说明</span><span class="sxs-lookup"><span data-stu-id="7d5e3-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="7d5e3-110">usersRegisteredByFeature</span><span class="sxs-lookup"><span data-stu-id="7d5e3-110">usersRegisteredByFeature</span></span>](../api/authenticationmethodsroot-usersregisteredbyfeature.md) | <span data-ttu-id="7d5e3-111">userRegistrationFeatureSummary</span><span class="sxs-lookup"><span data-stu-id="7d5e3-111">userRegistrationFeatureSummary</span></span> | <span data-ttu-id="7d5e3-112">获取能够进行多重身份验证、密码Self-Service密码重置和无密码身份验证的用户数。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-112">Get the number of users capable of Multi-Factor Authentication, Self-Service Password Reset, and Passwordless authentication.</span></span> |

## <a name="properties"></a><span data-ttu-id="7d5e3-113">属性</span><span class="sxs-lookup"><span data-stu-id="7d5e3-113">Properties</span></span>
|<span data-ttu-id="7d5e3-114">属性</span><span class="sxs-lookup"><span data-stu-id="7d5e3-114">Property</span></span>|<span data-ttu-id="7d5e3-115">类型</span><span class="sxs-lookup"><span data-stu-id="7d5e3-115">Type</span></span>|<span data-ttu-id="7d5e3-116">说明</span><span class="sxs-lookup"><span data-stu-id="7d5e3-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d5e3-117">totalUserCount</span><span class="sxs-lookup"><span data-stu-id="7d5e3-117">totalUserCount</span></span>|<span data-ttu-id="7d5e3-118">Int64</span><span class="sxs-lookup"><span data-stu-id="7d5e3-118">Int64</span></span>|<span data-ttu-id="7d5e3-119">用户帐户总数，不包括被阻止的帐户</span><span class="sxs-lookup"><span data-stu-id="7d5e3-119">Total number of users accounts, excluding those that are blocked</span></span>|
|<span data-ttu-id="7d5e3-120">userRegistrationFeatureCounts</span><span class="sxs-lookup"><span data-stu-id="7d5e3-120">userRegistrationFeatureCounts</span></span>|<span data-ttu-id="7d5e3-121">[userRegistrationFeatureCount](../resources/userregistrationfeaturecount.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7d5e3-121">[userRegistrationFeatureCount](../resources/userregistrationfeaturecount.md) collection</span></span>|<span data-ttu-id="7d5e3-122">注册或能够进行多重身份验证、密码重置Self-Service无密码身份验证的用户数量。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-122">Number of users registered or capable for Multi-Factor Authentication, Self-Service Password Reset and Passwordless Authentication.</span></span>|
|<span data-ttu-id="7d5e3-123">userRoles</span><span class="sxs-lookup"><span data-stu-id="7d5e3-123">userRoles</span></span>|<span data-ttu-id="7d5e3-124">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="7d5e3-124">includedUserRoles</span></span>|<span data-ttu-id="7d5e3-125">用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-125">User role type.</span></span> <span data-ttu-id="7d5e3-126">可取值为：`all`、`privilegedAdmin`、`admin`、`user`。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-126">Possible values are: `all`, `privilegedAdmin`, `admin`, `user`.</span></span>|
|<span data-ttu-id="7d5e3-127">userTypes</span><span class="sxs-lookup"><span data-stu-id="7d5e3-127">userTypes</span></span>|<span data-ttu-id="7d5e3-128">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="7d5e3-128">includedUserTypes</span></span>|<span data-ttu-id="7d5e3-129">用户类型。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-129">User type.</span></span> <span data-ttu-id="7d5e3-130">可取值为：`all`、`member`、`guest`。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-130">Possible values are: `all`, `member`, `guest`.</span></span>|

<span data-ttu-id="7d5e3-131">该值 `privilegedAdmin` 由以下特权管理员角色组成：</span><span class="sxs-lookup"><span data-stu-id="7d5e3-131">The value `privilegedAdmin` consists of the following privileged admin roles:</span></span>

* <span data-ttu-id="7d5e3-132">全局管理员</span><span class="sxs-lookup"><span data-stu-id="7d5e3-132">Global admin</span></span>
* <span data-ttu-id="7d5e3-133">安全管理员</span><span class="sxs-lookup"><span data-stu-id="7d5e3-133">Security admin</span></span>
* <span data-ttu-id="7d5e3-134">条件访问管理员</span><span class="sxs-lookup"><span data-stu-id="7d5e3-134">Conditional Access admin</span></span>
* <span data-ttu-id="7d5e3-135">Exchange 管理员</span><span class="sxs-lookup"><span data-stu-id="7d5e3-135">Exchange admin</span></span>
* <span data-ttu-id="7d5e3-136">SharePoint 管理员</span><span class="sxs-lookup"><span data-stu-id="7d5e3-136">SharePoint admin</span></span>
* <span data-ttu-id="7d5e3-137">支持管理员</span><span class="sxs-lookup"><span data-stu-id="7d5e3-137">Helpdesk admin</span></span>
* <span data-ttu-id="7d5e3-138">帐务管理员</span><span class="sxs-lookup"><span data-stu-id="7d5e3-138">Billing admin</span></span>
* <span data-ttu-id="7d5e3-139">用户管理员</span><span class="sxs-lookup"><span data-stu-id="7d5e3-139">User admin</span></span>
* <span data-ttu-id="7d5e3-140">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="7d5e3-140">Authentication admin</span></span>

<span data-ttu-id="7d5e3-141">该值 `admin` 包括所有 Azure AD 管理员角色。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-141">The value `admin` includes all Azure AD admin roles.</span></span> 

## <a name="relationships"></a><span data-ttu-id="7d5e3-142">关系</span><span class="sxs-lookup"><span data-stu-id="7d5e3-142">Relationships</span></span>
<span data-ttu-id="7d5e3-143">无。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d5e3-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d5e3-144">JSON representation</span></span>
<span data-ttu-id="7d5e3-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d5e3-145">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationFeatureSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationFeatureSummary",
  "totalUserCount": "Integer",
  "userTypes": "String",
  "userRoles": "String",
  "userRegistrationFeatureCounts": [
    {
      "@odata.type": "microsoft.graph.userRegistrationFeatureCount"
    }
  ]
}
```
