---
title: userRegistrationMethodSummary 资源类型
description: 针对每种身份验证方法注册的用户数的摘要。
author: danielwood95
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 6ff9a079ddce0df5031eef2b1374ebb1d233d56d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132917"
---
# <a name="userregistrationmethodsummary-resource-type"></a><span data-ttu-id="f26b5-103">userRegistrationMethodSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="f26b5-103">userRegistrationMethodSummary resource type</span></span>

<span data-ttu-id="f26b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f26b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f26b5-105">针对每种身份验证方法注册的用户数的摘要。</span><span class="sxs-lookup"><span data-stu-id="f26b5-105">Summary of number of users registered for each authentication method.</span></span>

## <a name="methods"></a><span data-ttu-id="f26b5-106">方法</span><span class="sxs-lookup"><span data-stu-id="f26b5-106">Methods</span></span>

| <span data-ttu-id="f26b5-107">方法</span><span class="sxs-lookup"><span data-stu-id="f26b5-107">Method</span></span>       | <span data-ttu-id="f26b5-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f26b5-108">Return Type</span></span> | <span data-ttu-id="f26b5-109">说明</span><span class="sxs-lookup"><span data-stu-id="f26b5-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f26b5-110">usersRegisteredByMethod</span><span class="sxs-lookup"><span data-stu-id="f26b5-110">usersRegisteredByMethod</span></span>](../api/authenticationmethodsroot-usersregisteredbymethod.md) | <span data-ttu-id="f26b5-111">userRegistrationMethodSummary</span><span class="sxs-lookup"><span data-stu-id="f26b5-111">userRegistrationMethodSummary</span></span> | <span data-ttu-id="f26b5-112">获取每个身份验证方法注册的用户数。</span><span class="sxs-lookup"><span data-stu-id="f26b5-112">Get the number of users registered for each authentication method.</span></span> |

## <a name="properties"></a><span data-ttu-id="f26b5-113">属性</span><span class="sxs-lookup"><span data-stu-id="f26b5-113">Properties</span></span>
|<span data-ttu-id="f26b5-114">属性</span><span class="sxs-lookup"><span data-stu-id="f26b5-114">Property</span></span>|<span data-ttu-id="f26b5-115">类型</span><span class="sxs-lookup"><span data-stu-id="f26b5-115">Type</span></span>|<span data-ttu-id="f26b5-116">说明</span><span class="sxs-lookup"><span data-stu-id="f26b5-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f26b5-117">totalUserCount</span><span class="sxs-lookup"><span data-stu-id="f26b5-117">totalUserCount</span></span>|<span data-ttu-id="f26b5-118">Int64</span><span class="sxs-lookup"><span data-stu-id="f26b5-118">Int64</span></span>|<span data-ttu-id="f26b5-119">租户中的用户总数。</span><span class="sxs-lookup"><span data-stu-id="f26b5-119">Total number of users in the tenant.</span></span>|
|<span data-ttu-id="f26b5-120">userRegistrationMethodCounts</span><span class="sxs-lookup"><span data-stu-id="f26b5-120">userRegistrationMethodCounts</span></span>|<span data-ttu-id="f26b5-121">[userRegistrationMethodCount](../resources/userregistrationmethodcount.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f26b5-121">[userRegistrationMethodCount](../resources/userregistrationmethodcount.md) collection</span></span>|<span data-ttu-id="f26b5-122">为每种身份验证方法注册的用户数。</span><span class="sxs-lookup"><span data-stu-id="f26b5-122">Number of users registered for each authentication method.</span></span>|
|<span data-ttu-id="f26b5-123">userRoles</span><span class="sxs-lookup"><span data-stu-id="f26b5-123">userRoles</span></span>|<span data-ttu-id="f26b5-124">includedUserRoles</span><span class="sxs-lookup"><span data-stu-id="f26b5-124">includedUserRoles</span></span>|<span data-ttu-id="f26b5-125">用户角色类型。</span><span class="sxs-lookup"><span data-stu-id="f26b5-125">User role type.</span></span> <span data-ttu-id="f26b5-126">可取值为：`all`、`privilegedAdmin`、`admin`、`user`。</span><span class="sxs-lookup"><span data-stu-id="f26b5-126">Possible values are: `all`, `privilegedAdmin`, `admin`, `user`.</span></span>|
|<span data-ttu-id="f26b5-127">userTypes</span><span class="sxs-lookup"><span data-stu-id="f26b5-127">userTypes</span></span>|<span data-ttu-id="f26b5-128">includedUserTypes</span><span class="sxs-lookup"><span data-stu-id="f26b5-128">includedUserTypes</span></span>|<span data-ttu-id="f26b5-129">用户类型。</span><span class="sxs-lookup"><span data-stu-id="f26b5-129">User type.</span></span> <span data-ttu-id="f26b5-130">可取值为：`all`、`member`、`guest`。</span><span class="sxs-lookup"><span data-stu-id="f26b5-130">Possible values are: `all`, `member`, `guest`.</span></span>|

<span data-ttu-id="f26b5-131">该值 `privilegedAdmin` 由以下特权管理员角色组成：</span><span class="sxs-lookup"><span data-stu-id="f26b5-131">The value `privilegedAdmin` consists of the following privileged admin roles:</span></span>

* <span data-ttu-id="f26b5-132">全局管理员</span><span class="sxs-lookup"><span data-stu-id="f26b5-132">Global admin</span></span>
* <span data-ttu-id="f26b5-133">安全管理员</span><span class="sxs-lookup"><span data-stu-id="f26b5-133">Security admin</span></span>
* <span data-ttu-id="f26b5-134">条件访问管理员</span><span class="sxs-lookup"><span data-stu-id="f26b5-134">Conditional Access admin</span></span>
* <span data-ttu-id="f26b5-135">Exchange 管理员</span><span class="sxs-lookup"><span data-stu-id="f26b5-135">Exchange admin</span></span>
* <span data-ttu-id="f26b5-136">SharePoint 管理员</span><span class="sxs-lookup"><span data-stu-id="f26b5-136">SharePoint admin</span></span>
* <span data-ttu-id="f26b5-137">支持管理员</span><span class="sxs-lookup"><span data-stu-id="f26b5-137">Helpdesk admin</span></span>
* <span data-ttu-id="f26b5-138">帐务管理员</span><span class="sxs-lookup"><span data-stu-id="f26b5-138">Billing admin</span></span>
* <span data-ttu-id="f26b5-139">用户管理员</span><span class="sxs-lookup"><span data-stu-id="f26b5-139">User admin</span></span>
* <span data-ttu-id="f26b5-140">身份验证管理员</span><span class="sxs-lookup"><span data-stu-id="f26b5-140">Authentication admin</span></span>

<span data-ttu-id="f26b5-141">该值 `admin` 包括所有 Azure AD 管理员角色。</span><span class="sxs-lookup"><span data-stu-id="f26b5-141">The value `admin` includes all Azure AD admin roles.</span></span> 

## <a name="relationships"></a><span data-ttu-id="f26b5-142">关系</span><span class="sxs-lookup"><span data-stu-id="f26b5-142">Relationships</span></span>
<span data-ttu-id="f26b5-143">无。</span><span class="sxs-lookup"><span data-stu-id="f26b5-143">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f26b5-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f26b5-144">JSON representation</span></span>
<span data-ttu-id="f26b5-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f26b5-145">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationMethodSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationMethodSummary",
  "totalUserCount": "Integer",
  "userTypes": "String",
  "userRoles": "String",
  "userRegistrationMethodCounts": [
    {
      "@odata.type": "microsoft.graph.userRegistrationMethodCount"
    }
  ]
}
```
