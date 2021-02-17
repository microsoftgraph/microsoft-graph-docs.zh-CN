---
title: temporaryAccessPassAuthenticationMethodConfiguration 资源类型
description: 表示临时访问传递身份验证方法策略。
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9edb4038180a96d6878fcaf6770728a1befbca19
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272601"
---
# <a name="temporaryaccesspassauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="d4aa5-103">temporaryAccessPassAuthenticationMethodConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4aa5-103">temporaryAccessPassAuthenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="d4aa5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4aa5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4aa5-105">表示临时访问传递身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="d4aa5-105">Represents a Temporary Access Pass authentication methods policy.</span></span> <span data-ttu-id="d4aa5-106">身份验证方法策略定义配置设置以及允许使用身份验证方法的用户或组。</span><span class="sxs-lookup"><span data-stu-id="d4aa5-106">The Authentication methods policy defines the configuration settings and users or groups who are enabled to use the authentication method.</span></span>

## <a name="methods"></a><span data-ttu-id="d4aa5-107">Methods</span><span class="sxs-lookup"><span data-stu-id="d4aa5-107">Methods</span></span>
|<span data-ttu-id="d4aa5-108">方法</span><span class="sxs-lookup"><span data-stu-id="d4aa5-108">Method</span></span>|<span data-ttu-id="d4aa5-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d4aa5-109">Return type</span></span>|<span data-ttu-id="d4aa5-110">说明</span><span class="sxs-lookup"><span data-stu-id="d4aa5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d4aa5-111">获取</span><span class="sxs-lookup"><span data-stu-id="d4aa5-111">Get</span></span>](../api/temporaryaccesspassauthenticationmethodconfiguration-get.md)|[<span data-ttu-id="d4aa5-112">temporaryaccesspassauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="d4aa5-112">temporaryaccesspassauthenticationmethodconfiguration</span></span>](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|<span data-ttu-id="d4aa5-113">读取 **temporaryaccesspassauthenticationmethodconfiguration** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d4aa5-113">Read the properties and relationships of a **temporaryaccesspassauthenticationmethodconfiguration** object.</span></span>|
|[<span data-ttu-id="d4aa5-114">更新</span><span class="sxs-lookup"><span data-stu-id="d4aa5-114">Update</span></span>](../api/temporaryaccesspassauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="d4aa5-115">temporaryaccesspassauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="d4aa5-115">temporaryaccesspassauthenticationmethodconfiguration</span></span>](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|<span data-ttu-id="d4aa5-116">更新 **temporaryaccesspassauthenticationmethodconfiguration 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="d4aa5-116">Update the properties of a **temporaryaccesspassauthenticationmethodconfiguration** object.</span></span>|
|[<span data-ttu-id="d4aa5-117">删除</span><span class="sxs-lookup"><span data-stu-id="d4aa5-117">Delete</span></span>](../api/temporaryaccesspassauthenticationmethodconfiguration-delete.md)|<span data-ttu-id="d4aa5-118">无</span><span class="sxs-lookup"><span data-stu-id="d4aa5-118">None</span></span>|<span data-ttu-id="d4aa5-119">将 **temporaryaccesspassauthenticationmethodconfiguration** 对象还原到其默认配置。</span><span class="sxs-lookup"><span data-stu-id="d4aa5-119">Reverts the **temporaryaccesspassauthenticationmethodconfiguration** object to its default configuration.</span></span>|

## <a name="properties"></a><span data-ttu-id="d4aa5-120">属性</span><span class="sxs-lookup"><span data-stu-id="d4aa5-120">Properties</span></span>
|<span data-ttu-id="d4aa5-121">属性</span><span class="sxs-lookup"><span data-stu-id="d4aa5-121">Property</span></span>|<span data-ttu-id="d4aa5-122">类型</span><span class="sxs-lookup"><span data-stu-id="d4aa5-122">Type</span></span>|<span data-ttu-id="d4aa5-123">说明</span><span class="sxs-lookup"><span data-stu-id="d4aa5-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4aa5-124">id</span><span class="sxs-lookup"><span data-stu-id="d4aa5-124">id</span></span>|<span data-ttu-id="d4aa5-125">String</span><span class="sxs-lookup"><span data-stu-id="d4aa5-125">String</span></span>|<span data-ttu-id="d4aa5-126">身份验证方法策略标识符。</span><span class="sxs-lookup"><span data-stu-id="d4aa5-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="d4aa5-127">minimumLifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="d4aa5-127">minimumLifetimeInMinutes</span></span>|<span data-ttu-id="d4aa5-128">Int</span><span class="sxs-lookup"><span data-stu-id="d4aa5-128">Int</span></span>|<span data-ttu-id="d4aa5-129">在租户中创建的任何 temporaryAccessPass 的最小生存期（分钟）。</span><span class="sxs-lookup"><span data-stu-id="d4aa5-129">Minimum lifetime in minutes for any temporaryAccessPass created in the tenant.</span></span> <span data-ttu-id="d4aa5-130">值可以介于 10 到 43200 (等于 30 天) 。</span><span class="sxs-lookup"><span data-stu-id="d4aa5-130">Value can be between 10 and 43200 minutes (equivalent to 30 days).</span></span>|
|<span data-ttu-id="d4aa5-131">maximumLifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="d4aa5-131">maximumLifetimeInMinutes</span></span>|<span data-ttu-id="d4aa5-132">Int</span><span class="sxs-lookup"><span data-stu-id="d4aa5-132">Int</span></span>|<span data-ttu-id="d4aa5-133">在租户中创建的任何 temporaryAccessPass 的最大生存期（分钟）。</span><span class="sxs-lookup"><span data-stu-id="d4aa5-133">Maximum lifetime in minutes for any temporaryAccessPass created in the tenant.</span></span> <span data-ttu-id="d4aa5-134">值可以介于 10 到 43200 (等于 30 天) 。</span><span class="sxs-lookup"><span data-stu-id="d4aa5-134">Value can be between 10 and 43200 minutes (equivalent to 30 days).</span></span>|
|<span data-ttu-id="d4aa5-135">defaultLifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="d4aa5-135">defaultLifetimeInMinutes</span></span>|<span data-ttu-id="d4aa5-136">int</span><span class="sxs-lookup"><span data-stu-id="d4aa5-136">int</span></span>|<span data-ttu-id="d4aa5-137">临时AccessPass 的默认生存期（分钟）。</span><span class="sxs-lookup"><span data-stu-id="d4aa5-137">Default lifetime, in minutes, for a temporaryAccessPass.</span></span> <span data-ttu-id="d4aa5-138">值可以在 minimumLifetimeInMinutes 和 maximumLifetimeInMinutes 之间。</span><span class="sxs-lookup"><span data-stu-id="d4aa5-138">Value can be between the minimumLifetimeInMinutes and maximumLifetimeInMinutes.</span></span>|
|<span data-ttu-id="d4aa5-139">defaultLength</span><span class="sxs-lookup"><span data-stu-id="d4aa5-139">defaultLength</span></span>|<span data-ttu-id="d4aa5-140">int</span><span class="sxs-lookup"><span data-stu-id="d4aa5-140">int</span></span>|<span data-ttu-id="d4aa5-141">temporaryAccessPass 的默认长度（以字符表示）介于 8 到 48 个字符之间。</span><span class="sxs-lookup"><span data-stu-id="d4aa5-141">Default length, in characters, of a temporaryAccessPass, between 8 and 48 characters.</span></span>|
|<span data-ttu-id="d4aa5-142">isUsableOnce</span><span class="sxs-lookup"><span data-stu-id="d4aa5-142">isUsableOnce</span></span>|<span data-ttu-id="d4aa5-143">布尔值</span><span class="sxs-lookup"><span data-stu-id="d4aa5-143">Boolean</span></span>   |<span data-ttu-id="d4aa5-144">如果 `true` ，租户中所有通道将限制为一次使用。</span><span class="sxs-lookup"><span data-stu-id="d4aa5-144">If `true`, all the passes in the tenant will be restricted to one-time use.</span></span> <span data-ttu-id="d4aa5-145">If `false` ， passes in the tenant can be created to be one-time use or multiple time use.</span><span class="sxs-lookup"><span data-stu-id="d4aa5-145">If `false`, passes in the tenant can be created to be either one-time use or multiple time use.</span></span>|
|<span data-ttu-id="d4aa5-146">state</span><span class="sxs-lookup"><span data-stu-id="d4aa5-146">state</span></span>|<span data-ttu-id="d4aa5-147">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="d4aa5-147">authenticationMethodState</span></span>|<span data-ttu-id="d4aa5-148">可取值为：`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="d4aa5-148">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4aa5-149">关系</span><span class="sxs-lookup"><span data-stu-id="d4aa5-149">Relationships</span></span>
|<span data-ttu-id="d4aa5-150">关系</span><span class="sxs-lookup"><span data-stu-id="d4aa5-150">Relationship</span></span>|<span data-ttu-id="d4aa5-151">类型</span><span class="sxs-lookup"><span data-stu-id="d4aa5-151">Type</span></span>|<span data-ttu-id="d4aa5-152">说明</span><span class="sxs-lookup"><span data-stu-id="d4aa5-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4aa5-153">includeTargets</span><span class="sxs-lookup"><span data-stu-id="d4aa5-153">includeTargets</span></span>|<span data-ttu-id="d4aa5-154">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d4aa5-154">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="d4aa5-155">允许使用身份验证方法的用户或组的集合。</span><span class="sxs-lookup"><span data-stu-id="d4aa5-155">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4aa5-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4aa5-156">JSON representation</span></span>
<span data-ttu-id="d4aa5-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4aa5-157">The following is a JSON representation of the resource.</span></span>

``` json
{
  "@odata.type": "#microsoft.authMethodPolicy.temporaryAccessPassAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "defaultLifetimeInMinutes": "Integer",
  "defaultLength": "Integer",
  "minimumLifetimeInMinutes": "Integer",
  "maximumLifetimeInMinutes": "Integer",
  "isUsableOnce": "Boolean"
},
"includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
