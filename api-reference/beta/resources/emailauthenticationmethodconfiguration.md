---
title: emailAuthenticationMethodConfiguration 资源类型
description: 代表电子邮件 OTP 身份验证方法策略
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3e3e18973759d7f120dd0bd8e984c98568054960
ms.sourcegitcommit: d9c167f6be71bdb4a023c5ace2733b9854c846d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2020
ms.locfileid: "49617113"
---
# <a name="emailauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="fce05-103">emailAuthenticationMethodConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="fce05-103">emailAuthenticationMethodConfiguration resource type</span></span>

<span data-ttu-id="fce05-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fce05-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fce05-105">表示此租户的电子邮件 OTP 身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="fce05-105">Represents this tenant's email OTP authentication methods policy.</span></span> <span data-ttu-id="fce05-106">身份验证方法策略定义启用使用身份验证方法的配置设置和用户或组。</span><span class="sxs-lookup"><span data-stu-id="fce05-106">Authentication methods policies define configuration settings and users or groups who are enabled to use the authentication method.</span></span> <span data-ttu-id="fce05-107">租户的云本机用户可以使用电子邮件 OTP 进行自助密码重置，也可以在某些情况下由外部用户用于身份验证。</span><span class="sxs-lookup"><span data-stu-id="fce05-107">Email OTP may be used by the tenant's cloud-native users for self-service password reset, or by external users for authentication in some circumstances.</span></span>

## <a name="methods"></a><span data-ttu-id="fce05-108">方法</span><span class="sxs-lookup"><span data-stu-id="fce05-108">Methods</span></span>

|<span data-ttu-id="fce05-109">方法</span><span class="sxs-lookup"><span data-stu-id="fce05-109">Method</span></span>|<span data-ttu-id="fce05-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="fce05-110">Return type</span></span>|<span data-ttu-id="fce05-111">说明</span><span class="sxs-lookup"><span data-stu-id="fce05-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fce05-112">获取 emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="fce05-112">Get emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-get.md)|[<span data-ttu-id="fce05-113">emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="fce05-113">emailAuthenticationMethodConfiguration</span></span>](../resources/emailauthenticationmethodconfiguration.md)|<span data-ttu-id="fce05-114">读取 emailAuthenticationMethodConfiguration 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fce05-114">Read the properties and relationships of an emailAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="fce05-115">更新 emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="fce05-115">Update emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="fce05-116">emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="fce05-116">emailAuthenticationMethodConfiguration</span></span>](../resources/emailauthenticationmethodconfiguration.md)|<span data-ttu-id="fce05-117">更新 emailAuthenticationMethodConfiguration 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fce05-117">Update the properties of an emailAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="fce05-118">删除 emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="fce05-118">Delete emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-delete.md)|<span data-ttu-id="fce05-119">无</span><span class="sxs-lookup"><span data-stu-id="fce05-119">None</span></span>|<span data-ttu-id="fce05-120">删除一个 emailAuthenticationMethodConfiguration 对象。</span><span class="sxs-lookup"><span data-stu-id="fce05-120">Deletes an emailAuthenticationMethodConfiguration object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fce05-121">属性</span><span class="sxs-lookup"><span data-stu-id="fce05-121">Properties</span></span>

|<span data-ttu-id="fce05-122">属性</span><span class="sxs-lookup"><span data-stu-id="fce05-122">Property</span></span>|<span data-ttu-id="fce05-123">类型</span><span class="sxs-lookup"><span data-stu-id="fce05-123">Type</span></span>|<span data-ttu-id="fce05-124">说明</span><span class="sxs-lookup"><span data-stu-id="fce05-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fce05-125">id</span><span class="sxs-lookup"><span data-stu-id="fce05-125">id</span></span>|<span data-ttu-id="fce05-126">String</span><span class="sxs-lookup"><span data-stu-id="fce05-126">String</span></span>|<span data-ttu-id="fce05-127">身份验证方法策略标识符。</span><span class="sxs-lookup"><span data-stu-id="fce05-127">The authentication method policy identifier.</span></span> <span data-ttu-id="fce05-128">继承自 [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="fce05-128">Inherited from [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md).</span></span>|
|<span data-ttu-id="fce05-129">state</span><span class="sxs-lookup"><span data-stu-id="fce05-129">state</span></span>|<span data-ttu-id="fce05-130">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="fce05-130">authenticationMethodState</span></span>|<span data-ttu-id="fce05-131">指示是否启用此身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="fce05-131">Indicates whether this authentication method is enabled or not.</span></span> <span data-ttu-id="fce05-132">可取值为：`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="fce05-132">Possible values are: `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="fce05-133">allowExternalIdToUseEmailOtp</span><span class="sxs-lookup"><span data-stu-id="fce05-133">allowExternalIdToUseEmailOtp</span></span>|<span data-ttu-id="fce05-134">externalEmailOtpState</span><span class="sxs-lookup"><span data-stu-id="fce05-134">externalEmailOtpState</span></span>|<span data-ttu-id="fce05-135">确定外部用户是否可使用电子邮件 OTP 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="fce05-135">Determines whether email OTP is usable by external users for authentication.</span></span> <span data-ttu-id="fce05-136">可取值为：`default`、`enabled`、`disabled`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="fce05-136">Possible values are: `default`, `enabled`, `disabled`, `unknownFutureValue`.</span></span> <span data-ttu-id="fce05-137">`default`未使用公共预览版的状态中的租户将自动启用电子邮件 OTP （从3月2021开始）。</span><span class="sxs-lookup"><span data-stu-id="fce05-137">Tenants in the `default` state who did not use public preview will automatically have email OTP enabled beginning in March 2021.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fce05-138">关系</span><span class="sxs-lookup"><span data-stu-id="fce05-138">Relationships</span></span>

|<span data-ttu-id="fce05-139">关系</span><span class="sxs-lookup"><span data-stu-id="fce05-139">Relationship</span></span>|<span data-ttu-id="fce05-140">类型</span><span class="sxs-lookup"><span data-stu-id="fce05-140">Type</span></span>|<span data-ttu-id="fce05-141">说明</span><span class="sxs-lookup"><span data-stu-id="fce05-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fce05-142">includeTargets</span><span class="sxs-lookup"><span data-stu-id="fce05-142">includeTargets</span></span>|<span data-ttu-id="fce05-143">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fce05-143">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="fce05-144">启用使用身份验证方法的用户或组的集合。</span><span class="sxs-lookup"><span data-stu-id="fce05-144">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fce05-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fce05-145">JSON representation</span></span>

<span data-ttu-id="fce05-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fce05-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailAuthenticationMethodConfiguration",
  "baseType": "microsoft.graph.authenticationMethodConfiguration",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.emailAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "allowExternalIdToUseEmailOtp": "String",
  "includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
