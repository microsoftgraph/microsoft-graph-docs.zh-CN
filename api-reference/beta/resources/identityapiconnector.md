---
title: identityApiConnector 资源类型
description: 表示 Azure Active Directory 租户中的 API 连接器。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6098b146b5117332df36b76adcbce95698d6041d
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720160"
---
# <a name="identityapiconnector-resource-type"></a><span data-ttu-id="25d54-103">identityApiConnector 资源类型</span><span class="sxs-lookup"><span data-stu-id="25d54-103">identityApiConnector resource type</span></span>

<span data-ttu-id="25d54-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25d54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25d54-105">表示 Azure Active Directory 中的 API (Azure AD) 和 Azure AD B2C 租户。</span><span class="sxs-lookup"><span data-stu-id="25d54-105">Represents API connectors in an Azure Active Directory (Azure AD) and Azure AD B2C tenants.</span></span>

<span data-ttu-id="25d54-106">Azure AD 外部标识自助注册和 Azure AD B2C 注册用户流中使用的 API 连接器允许你在执行用户流期间调用 API。</span><span class="sxs-lookup"><span data-stu-id="25d54-106">An API connector used in your Azure AD External Identities self-service sign-up and Azure AD B2C sign-up user flows allows you to call an API during the execution of the user flow.</span></span> <span data-ttu-id="25d54-107">API 连接器提供调用 API 所需的信息，包括终结点 URL 和身份验证。</span><span class="sxs-lookup"><span data-stu-id="25d54-107">An API connector provides the information needed to call an API including an endpoint URL and authentication.</span></span> <span data-ttu-id="25d54-108">API 连接器可在用户流中的特定步骤使用，以影响用户流的执行。</span><span class="sxs-lookup"><span data-stu-id="25d54-108">An API connector can be used at a specific step in a user flow to affect the execution of the user flow.</span></span> <span data-ttu-id="25d54-109">例如，API 响应可以阻止用户注册、显示输入验证错误或覆盖用户收集的属性。</span><span class="sxs-lookup"><span data-stu-id="25d54-109">For example, the API response can block a user from signing up, show an input validation error, or overwrite user collected attributes.</span></span>

<span data-ttu-id="25d54-110">使用 [b2xIdentityUserFlow](b2xidentityuserflow.md) API 从外部标识自助注册用户流使用 API 连接器。</span><span class="sxs-lookup"><span data-stu-id="25d54-110">Use the [b2xIdentityUserFlow](b2xidentityuserflow.md) API to use an API connector from an External Identities self-service sign-up user flow.</span></span>

## <a name="methods"></a><span data-ttu-id="25d54-111">方法</span><span class="sxs-lookup"><span data-stu-id="25d54-111">Methods</span></span>

|<span data-ttu-id="25d54-112">方法</span><span class="sxs-lookup"><span data-stu-id="25d54-112">Method</span></span>|<span data-ttu-id="25d54-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="25d54-113">Return type</span></span>|<span data-ttu-id="25d54-114">Description</span><span class="sxs-lookup"><span data-stu-id="25d54-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="25d54-115">List</span><span class="sxs-lookup"><span data-stu-id="25d54-115">List</span></span>](../api/identityapiconnector-list.md)|<span data-ttu-id="25d54-116">[identityApiConnector](identityapiconnector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25d54-116">[identityApiConnector](identityapiconnector.md) collection</span></span>| <span data-ttu-id="25d54-117">获取 API 连接器列表</span><span class="sxs-lookup"><span data-stu-id="25d54-117">Get a list of API connectors</span></span>|
|[<span data-ttu-id="25d54-118">创建</span><span class="sxs-lookup"><span data-stu-id="25d54-118">Create</span></span>](../api/identityapiconnector-create.md)|[<span data-ttu-id="25d54-119">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="25d54-119">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="25d54-120">创建新的 API 连接器。</span><span class="sxs-lookup"><span data-stu-id="25d54-120">Create a new API connector.</span></span> |
|[<span data-ttu-id="25d54-121">获取</span><span class="sxs-lookup"><span data-stu-id="25d54-121">Get</span></span>](../api/identityapiconnector-get.md)|[<span data-ttu-id="25d54-122">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="25d54-122">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="25d54-123">读取 [identityApiConnector 对象](../resources/identityapiconnector.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="25d54-123">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>|
|[<span data-ttu-id="25d54-124">更新</span><span class="sxs-lookup"><span data-stu-id="25d54-124">Update</span></span>](../api/identityapiconnector-update.md)|[<span data-ttu-id="25d54-125">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="25d54-125">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="25d54-126">更新 API 连接器的属性。</span><span class="sxs-lookup"><span data-stu-id="25d54-126">Update the properties of an API connector.</span></span>|
|[<span data-ttu-id="25d54-127">删除</span><span class="sxs-lookup"><span data-stu-id="25d54-127">Delete</span></span>](../api/identityapiconnector-delete.md)|<span data-ttu-id="25d54-128">无</span><span class="sxs-lookup"><span data-stu-id="25d54-128">None</span></span>|<span data-ttu-id="25d54-129">删除 API 连接器。</span><span class="sxs-lookup"><span data-stu-id="25d54-129">Delete an API connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="25d54-130">属性</span><span class="sxs-lookup"><span data-stu-id="25d54-130">Properties</span></span>

|<span data-ttu-id="25d54-131">属性</span><span class="sxs-lookup"><span data-stu-id="25d54-131">Property</span></span>|<span data-ttu-id="25d54-132">类型</span><span class="sxs-lookup"><span data-stu-id="25d54-132">Type</span></span>|<span data-ttu-id="25d54-133">说明</span><span class="sxs-lookup"><span data-stu-id="25d54-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25d54-134">id</span><span class="sxs-lookup"><span data-stu-id="25d54-134">id</span></span>|<span data-ttu-id="25d54-135">String</span><span class="sxs-lookup"><span data-stu-id="25d54-135">String</span></span>|<span data-ttu-id="25d54-136">API 连接器的随机生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="25d54-136">The randomly generated ID of the API connector.</span></span> |
|<span data-ttu-id="25d54-137">displayName</span><span class="sxs-lookup"><span data-stu-id="25d54-137">displayName</span></span>|<span data-ttu-id="25d54-138">String</span><span class="sxs-lookup"><span data-stu-id="25d54-138">String</span></span>| <span data-ttu-id="25d54-139">API 连接器的名称。</span><span class="sxs-lookup"><span data-stu-id="25d54-139">The name of the API connector.</span></span> |
|<span data-ttu-id="25d54-140">targetUrl</span><span class="sxs-lookup"><span data-stu-id="25d54-140">targetUrl</span></span>|<span data-ttu-id="25d54-141">String</span><span class="sxs-lookup"><span data-stu-id="25d54-141">String</span></span>| <span data-ttu-id="25d54-142">要调用的 API 终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="25d54-142">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="25d54-143">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="25d54-143">authenticationConfiguration</span></span>|[<span data-ttu-id="25d54-144">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="25d54-144">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="25d54-145">描述用于调用 API 的身份验证配置详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="25d54-145">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="25d54-146">目前 [仅](basicauthentication.md) 支持基本身份验证。</span><span class="sxs-lookup"><span data-stu-id="25d54-146">Only [Basic authentication](basicauthentication.md) is supported at this time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25d54-147">关系</span><span class="sxs-lookup"><span data-stu-id="25d54-147">Relationships</span></span>

<span data-ttu-id="25d54-148">无。</span><span class="sxs-lookup"><span data-stu-id="25d54-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="25d54-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="25d54-149">JSON representation</span></span>

<span data-ttu-id="25d54-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25d54-150">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityApiConnector",
  "baseType": "",
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
