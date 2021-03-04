---
title: identityApiConnector 资源类型
description: 表示 Azure Active Directory 租户中的 API 连接器。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: a267fdb60dfcbcbbadfe75c65d49137f46425434
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443025"
---
# <a name="identityapiconnector-resource-type"></a><span data-ttu-id="6dd0e-103">identityApiConnector 资源类型</span><span class="sxs-lookup"><span data-stu-id="6dd0e-103">identityApiConnector resource type</span></span>

<span data-ttu-id="6dd0e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6dd0e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dd0e-105">表示 Azure Active Directory (Azure AD) 和 Azure AD B2C 租户中的 API 连接器。</span><span class="sxs-lookup"><span data-stu-id="6dd0e-105">Represents API connectors in an Azure Active Directory (Azure AD) and Azure AD B2C tenants.</span></span>

<span data-ttu-id="6dd0e-106">Azure AD 外部标识自助注册和 Azure AD B2C 注册用户流中使用的 API 连接器允许你在执行用户流期间调用 API。</span><span class="sxs-lookup"><span data-stu-id="6dd0e-106">An API connector used in your Azure AD External Identities self-service sign-up and Azure AD B2C sign-up user flows allows you to call an API during the execution of the user flow.</span></span> <span data-ttu-id="6dd0e-107">API 连接器提供调用 API 所需的信息，包括终结点 URL 和身份验证。</span><span class="sxs-lookup"><span data-stu-id="6dd0e-107">An API connector provides the information needed to call an API including an endpoint URL and authentication.</span></span> <span data-ttu-id="6dd0e-108">API 连接器可在用户流中的特定步骤使用，以影响用户流的执行。</span><span class="sxs-lookup"><span data-stu-id="6dd0e-108">An API connector can be used at a specific step in a user flow to affect the execution of the user flow.</span></span> <span data-ttu-id="6dd0e-109">例如，API 响应可以阻止用户注册、显示输入验证错误或覆盖用户收集的属性。</span><span class="sxs-lookup"><span data-stu-id="6dd0e-109">For example, the API response can block a user from signing up, show an input validation error, or overwrite user collected attributes.</span></span>

<span data-ttu-id="6dd0e-110">使用 [b2xIdentityUserFlow](b2xidentityuserflow.md) API 从外部标识自助注册用户流使用 API 连接器。</span><span class="sxs-lookup"><span data-stu-id="6dd0e-110">Use the [b2xIdentityUserFlow](b2xidentityuserflow.md) API to use an API connector from an External Identities self-service sign-up user flow.</span></span>

## <a name="methods"></a><span data-ttu-id="6dd0e-111">Methods</span><span class="sxs-lookup"><span data-stu-id="6dd0e-111">Methods</span></span>

|<span data-ttu-id="6dd0e-112">方法</span><span class="sxs-lookup"><span data-stu-id="6dd0e-112">Method</span></span>|<span data-ttu-id="6dd0e-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="6dd0e-113">Return type</span></span>|<span data-ttu-id="6dd0e-114">Description</span><span class="sxs-lookup"><span data-stu-id="6dd0e-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6dd0e-115">List</span><span class="sxs-lookup"><span data-stu-id="6dd0e-115">List</span></span>](../api/identityapiconnector-list.md)|<span data-ttu-id="6dd0e-116">[identityApiConnector](identityapiconnector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6dd0e-116">[identityApiConnector](identityapiconnector.md) collection</span></span>| <span data-ttu-id="6dd0e-117">获取 API 连接器列表</span><span class="sxs-lookup"><span data-stu-id="6dd0e-117">Get a list of API connectors</span></span>|
|[<span data-ttu-id="6dd0e-118">创建</span><span class="sxs-lookup"><span data-stu-id="6dd0e-118">Create</span></span>](../api/identityapiconnector-create.md)|[<span data-ttu-id="6dd0e-119">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="6dd0e-119">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="6dd0e-120">创建新的 API 连接器。</span><span class="sxs-lookup"><span data-stu-id="6dd0e-120">Create a new API connector.</span></span> |
|[<span data-ttu-id="6dd0e-121">获取</span><span class="sxs-lookup"><span data-stu-id="6dd0e-121">Get</span></span>](../api/identityapiconnector-get.md)|[<span data-ttu-id="6dd0e-122">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="6dd0e-122">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="6dd0e-123">读取 [identityApiConnector 对象](../resources/identityapiconnector.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="6dd0e-123">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>|
|[<span data-ttu-id="6dd0e-124">更新</span><span class="sxs-lookup"><span data-stu-id="6dd0e-124">Update</span></span>](../api/identityapiconnector-update.md)|[<span data-ttu-id="6dd0e-125">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="6dd0e-125">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="6dd0e-126">更新 API 连接器的属性。</span><span class="sxs-lookup"><span data-stu-id="6dd0e-126">Update the properties of an API connector.</span></span>|
|[<span data-ttu-id="6dd0e-127">删除</span><span class="sxs-lookup"><span data-stu-id="6dd0e-127">Delete</span></span>](../api/identityapiconnector-delete.md)|<span data-ttu-id="6dd0e-128">无</span><span class="sxs-lookup"><span data-stu-id="6dd0e-128">None</span></span>|<span data-ttu-id="6dd0e-129">删除 API 连接器。</span><span class="sxs-lookup"><span data-stu-id="6dd0e-129">Delete an API connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="6dd0e-130">属性</span><span class="sxs-lookup"><span data-stu-id="6dd0e-130">Properties</span></span>

|<span data-ttu-id="6dd0e-131">属性</span><span class="sxs-lookup"><span data-stu-id="6dd0e-131">Property</span></span>|<span data-ttu-id="6dd0e-132">类型</span><span class="sxs-lookup"><span data-stu-id="6dd0e-132">Type</span></span>|<span data-ttu-id="6dd0e-133">说明</span><span class="sxs-lookup"><span data-stu-id="6dd0e-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6dd0e-134">id</span><span class="sxs-lookup"><span data-stu-id="6dd0e-134">id</span></span>|<span data-ttu-id="6dd0e-135">String</span><span class="sxs-lookup"><span data-stu-id="6dd0e-135">String</span></span>|<span data-ttu-id="6dd0e-136">API 连接器的随机生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="6dd0e-136">The randomly generated ID of the API connector.</span></span> |
|<span data-ttu-id="6dd0e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="6dd0e-137">displayName</span></span>|<span data-ttu-id="6dd0e-138">String</span><span class="sxs-lookup"><span data-stu-id="6dd0e-138">String</span></span>| <span data-ttu-id="6dd0e-139">API 连接器的名称。</span><span class="sxs-lookup"><span data-stu-id="6dd0e-139">The name of the API connector.</span></span> |
|<span data-ttu-id="6dd0e-140">targetUrl</span><span class="sxs-lookup"><span data-stu-id="6dd0e-140">targetUrl</span></span>|<span data-ttu-id="6dd0e-141">String</span><span class="sxs-lookup"><span data-stu-id="6dd0e-141">String</span></span>| <span data-ttu-id="6dd0e-142">要调用的 API 终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="6dd0e-142">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="6dd0e-143">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="6dd0e-143">authenticationConfiguration</span></span>|[<span data-ttu-id="6dd0e-144">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="6dd0e-144">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="6dd0e-145">描述用于调用 API 的身份验证配置详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="6dd0e-145">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="6dd0e-146">目前 [仅](basicauthentication.md) 支持基本身份验证。</span><span class="sxs-lookup"><span data-stu-id="6dd0e-146">Only [Basic authentication](basicauthentication.md) is supported at this time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6dd0e-147">关系</span><span class="sxs-lookup"><span data-stu-id="6dd0e-147">Relationships</span></span>

<span data-ttu-id="6dd0e-148">无。</span><span class="sxs-lookup"><span data-stu-id="6dd0e-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6dd0e-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6dd0e-149">JSON representation</span></span>

<span data-ttu-id="6dd0e-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6dd0e-150">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityApiConnector",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityApiConnector",
  "id": "String (identifier)",
  "displayName": "String",
  "targetUrl": "String",
  "authenticationConfiguration": {
    "@odata.type": "microsoft.graph.apiAuthenticationConfigurationBase"
  }
}
```
