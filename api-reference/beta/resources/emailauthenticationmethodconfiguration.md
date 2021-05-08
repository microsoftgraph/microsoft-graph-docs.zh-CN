---
title: emailAuthenticationMethodConfiguration 资源类型
description: 代表电子邮件 OTP 身份验证方法策略
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1f85db08d4502df6cc3a928d2d56761b33dcc6d8
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232044"
---
# <a name="emailauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="ab5b7-103">emailAuthenticationMethodConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab5b7-103">emailAuthenticationMethodConfiguration resource type</span></span>

<span data-ttu-id="ab5b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab5b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab5b7-105">表示此租户的电子邮件 OTP 身份验证方法策略。</span><span class="sxs-lookup"><span data-stu-id="ab5b7-105">Represents this tenant's email OTP authentication methods policy.</span></span> <span data-ttu-id="ab5b7-106">身份验证方法策略定义配置设置以及能够使用身份验证方法的用户或组。</span><span class="sxs-lookup"><span data-stu-id="ab5b7-106">Authentication methods policies define configuration settings and users or groups who are enabled to use the authentication method.</span></span> <span data-ttu-id="ab5b7-107">租户的云本机用户可能会使用电子邮件 OTP 进行自助服务密码重置，或者外部用户在邀请兑换和自助注册用户流中的特定应用期间进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="ab5b7-107">Email OTP may be used by the tenant's cloud-native users for self-service password reset, or by external users for authentication during invitation redemption and self-service sign-up for specific apps in user flows.</span></span>

## <a name="methods"></a><span data-ttu-id="ab5b7-108">方法</span><span class="sxs-lookup"><span data-stu-id="ab5b7-108">Methods</span></span>

|<span data-ttu-id="ab5b7-109">方法</span><span class="sxs-lookup"><span data-stu-id="ab5b7-109">Method</span></span>|<span data-ttu-id="ab5b7-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ab5b7-110">Return type</span></span>|<span data-ttu-id="ab5b7-111">说明</span><span class="sxs-lookup"><span data-stu-id="ab5b7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ab5b7-112">获取 emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ab5b7-112">Get emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-get.md)|[<span data-ttu-id="ab5b7-113">emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ab5b7-113">emailAuthenticationMethodConfiguration</span></span>](../resources/emailauthenticationmethodconfiguration.md)|<span data-ttu-id="ab5b7-114">读取 emailAuthenticationMethodConfiguration 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ab5b7-114">Read the properties and relationships of an emailAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="ab5b7-115">更新 emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ab5b7-115">Update emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="ab5b7-116">emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ab5b7-116">emailAuthenticationMethodConfiguration</span></span>](../resources/emailauthenticationmethodconfiguration.md)|<span data-ttu-id="ab5b7-117">更新 emailAuthenticationMethodConfiguration 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ab5b7-117">Update the properties of an emailAuthenticationMethodConfiguration object.</span></span>|
|[<span data-ttu-id="ab5b7-118">删除 emailAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="ab5b7-118">Delete emailAuthenticationMethodConfiguration</span></span>](../api/emailauthenticationmethodconfiguration-delete.md)|<span data-ttu-id="ab5b7-119">无</span><span class="sxs-lookup"><span data-stu-id="ab5b7-119">None</span></span>|<span data-ttu-id="ab5b7-120">删除 emailAuthenticationMethodConfiguration 对象。</span><span class="sxs-lookup"><span data-stu-id="ab5b7-120">Deletes an emailAuthenticationMethodConfiguration object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ab5b7-121">属性</span><span class="sxs-lookup"><span data-stu-id="ab5b7-121">Properties</span></span>

|<span data-ttu-id="ab5b7-122">属性</span><span class="sxs-lookup"><span data-stu-id="ab5b7-122">Property</span></span>|<span data-ttu-id="ab5b7-123">类型</span><span class="sxs-lookup"><span data-stu-id="ab5b7-123">Type</span></span>|<span data-ttu-id="ab5b7-124">说明</span><span class="sxs-lookup"><span data-stu-id="ab5b7-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab5b7-125">id</span><span class="sxs-lookup"><span data-stu-id="ab5b7-125">id</span></span>|<span data-ttu-id="ab5b7-126">String</span><span class="sxs-lookup"><span data-stu-id="ab5b7-126">String</span></span>|<span data-ttu-id="ab5b7-127">身份验证方法策略标识符。</span><span class="sxs-lookup"><span data-stu-id="ab5b7-127">The authentication method policy identifier.</span></span> <span data-ttu-id="ab5b7-128">继承自 [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="ab5b7-128">Inherited from [authenticationMethodConfiguration](../resources/authenticationmethodconfiguration.md).</span></span>|
|<span data-ttu-id="ab5b7-129">状态</span><span class="sxs-lookup"><span data-stu-id="ab5b7-129">state</span></span>|<span data-ttu-id="ab5b7-130">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="ab5b7-130">authenticationMethodState</span></span>|<span data-ttu-id="ab5b7-131">指示是否启用此身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="ab5b7-131">Indicates whether this authentication method is enabled or not.</span></span> <span data-ttu-id="ab5b7-132">可取值为：`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="ab5b7-132">Possible values are: `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="ab5b7-133">allowExternalIdToUseEmailOtp</span><span class="sxs-lookup"><span data-stu-id="ab5b7-133">allowExternalIdToUseEmailOtp</span></span>|<span data-ttu-id="ab5b7-134">externalEmailOtpState</span><span class="sxs-lookup"><span data-stu-id="ab5b7-134">externalEmailOtpState</span></span>|<span data-ttu-id="ab5b7-135">确定外部用户是否可以使用电子邮件 OTP 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="ab5b7-135">Determines whether email OTP is usable by external users for authentication.</span></span> <span data-ttu-id="ab5b7-136">可取值为：`default`、`enabled`、`disabled`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="ab5b7-136">Possible values are: `default`, `enabled`, `disabled`, `unknownFutureValue`.</span></span> <span data-ttu-id="ab5b7-137">从 2021 年 10 开始，不使用公共预览的州中的租户将自动启用电子邮件 `default` OTP。</span><span class="sxs-lookup"><span data-stu-id="ab5b7-137">Tenants in the `default` state who did not use public preview will automatically have email OTP enabled beginning in October 2021.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab5b7-138">关系</span><span class="sxs-lookup"><span data-stu-id="ab5b7-138">Relationships</span></span>

|<span data-ttu-id="ab5b7-139">关系</span><span class="sxs-lookup"><span data-stu-id="ab5b7-139">Relationship</span></span>|<span data-ttu-id="ab5b7-140">类型</span><span class="sxs-lookup"><span data-stu-id="ab5b7-140">Type</span></span>|<span data-ttu-id="ab5b7-141">说明</span><span class="sxs-lookup"><span data-stu-id="ab5b7-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab5b7-142">includeTargets</span><span class="sxs-lookup"><span data-stu-id="ab5b7-142">includeTargets</span></span>|<span data-ttu-id="ab5b7-143">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ab5b7-143">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="ab5b7-144">允许使用身份验证方法的用户或组的集合。</span><span class="sxs-lookup"><span data-stu-id="ab5b7-144">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ab5b7-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab5b7-145">JSON representation</span></span>

<span data-ttu-id="ab5b7-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab5b7-146">The following is a JSON representation of the resource.</span></span>
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
