---
title: identityApiConnector 资源类型
description: 表示 Azure Active Directory 租户中的 API 连接器。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f7ecb96a9ca2f4397c1f0ee52908a7802374df0f
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508083"
---
# <a name="identityapiconnector-resource-type"></a><span data-ttu-id="42261-103">identityApiConnector 资源类型</span><span class="sxs-lookup"><span data-stu-id="42261-103">identityApiConnector resource type</span></span>

<span data-ttu-id="42261-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="42261-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42261-105">表示 Azure AD 租户和 Azure AD (Azure AD) Azure Active Directory 中的 API 连接器。</span><span class="sxs-lookup"><span data-stu-id="42261-105">Represents API connectors in an Azure Active Directory (Azure AD) and Azure AD B2C tenants.</span></span>

<span data-ttu-id="42261-106">Azure AD 外部标识自助注册中使用的 API 连接器和 Azure AD B2C 注册用户流允许你在执行用户流期间调用 API。</span><span class="sxs-lookup"><span data-stu-id="42261-106">An API connector used in your Azure AD External Identities self-service sign-up and Azure AD B2C sign-up user flows allows you to call an API during the execution of the user flow.</span></span> <span data-ttu-id="42261-107">API 连接器提供调用 API 时需要的信息，包括终结点 URL 和身份验证。</span><span class="sxs-lookup"><span data-stu-id="42261-107">An API connector provides the information needed to call an API including an endpoint URL and authentication.</span></span> <span data-ttu-id="42261-108">API 连接器可在用户流中的特定步骤使用，以影响用户流的执行。</span><span class="sxs-lookup"><span data-stu-id="42261-108">An API connector can be used at a specific step in a user flow to affect the execution of the user flow.</span></span> <span data-ttu-id="42261-109">例如，API 响应可以阻止用户注册、显示输入验证错误或覆盖用户收集的属性。</span><span class="sxs-lookup"><span data-stu-id="42261-109">For example, the API response can block a user from signing up, show an input validation error, or overwrite user collected attributes.</span></span>

<span data-ttu-id="42261-110">使用 [b2xIdentityUserFlow](b2xidentityuserflow.md) API 从外部标识自助注册用户流使用 API 连接器。</span><span class="sxs-lookup"><span data-stu-id="42261-110">Use the [b2xIdentityUserFlow](b2xidentityuserflow.md) API to use an API connector from an External Identities self-service sign-up user flow.</span></span>

## <a name="methods"></a><span data-ttu-id="42261-111">方法</span><span class="sxs-lookup"><span data-stu-id="42261-111">Methods</span></span>

|<span data-ttu-id="42261-112">方法</span><span class="sxs-lookup"><span data-stu-id="42261-112">Method</span></span>|<span data-ttu-id="42261-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="42261-113">Return type</span></span>|<span data-ttu-id="42261-114">Description</span><span class="sxs-lookup"><span data-stu-id="42261-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="42261-115">List</span><span class="sxs-lookup"><span data-stu-id="42261-115">List</span></span>](../api/identityapiconnector-list.md)|<span data-ttu-id="42261-116">[identityApiConnector](identityapiconnector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="42261-116">[identityApiConnector](identityapiconnector.md) collection</span></span>| <span data-ttu-id="42261-117">获取 API 连接器列表</span><span class="sxs-lookup"><span data-stu-id="42261-117">Get a list of API connectors</span></span>|
|[<span data-ttu-id="42261-118">创建</span><span class="sxs-lookup"><span data-stu-id="42261-118">Create</span></span>](../api/identityapiconnector-create.md)|[<span data-ttu-id="42261-119">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="42261-119">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="42261-120">创建新的 API 连接器。</span><span class="sxs-lookup"><span data-stu-id="42261-120">Create a new API connector.</span></span> |
|[<span data-ttu-id="42261-121">获取</span><span class="sxs-lookup"><span data-stu-id="42261-121">Get</span></span>](../api/identityapiconnector-get.md)|[<span data-ttu-id="42261-122">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="42261-122">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="42261-123">读取 [identityApiConnector 对象](../resources/identityapiconnector.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="42261-123">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>|
|[<span data-ttu-id="42261-124">更新</span><span class="sxs-lookup"><span data-stu-id="42261-124">Update</span></span>](../api/identityapiconnector-update.md)|[<span data-ttu-id="42261-125">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="42261-125">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="42261-126">更新 API 连接器的属性。</span><span class="sxs-lookup"><span data-stu-id="42261-126">Update the properties of an API connector.</span></span>|
|[<span data-ttu-id="42261-127">上载客户端证书</span><span class="sxs-lookup"><span data-stu-id="42261-127">Upload client certificate</span></span>](../api/identityapiconnector-uploadclientcertificate.md)|[<span data-ttu-id="42261-128">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="42261-128">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="42261-129">上载客户端证书以用于身份验证。</span><span class="sxs-lookup"><span data-stu-id="42261-129">Upload a client certificate to use for authentication.</span></span>|
|[<span data-ttu-id="42261-130">删除</span><span class="sxs-lookup"><span data-stu-id="42261-130">Delete</span></span>](../api/identityapiconnector-delete.md)|<span data-ttu-id="42261-131">无</span><span class="sxs-lookup"><span data-stu-id="42261-131">None</span></span>|<span data-ttu-id="42261-132">删除 API 连接器。</span><span class="sxs-lookup"><span data-stu-id="42261-132">Delete an API connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="42261-133">属性</span><span class="sxs-lookup"><span data-stu-id="42261-133">Properties</span></span>

|<span data-ttu-id="42261-134">属性</span><span class="sxs-lookup"><span data-stu-id="42261-134">Property</span></span>|<span data-ttu-id="42261-135">类型</span><span class="sxs-lookup"><span data-stu-id="42261-135">Type</span></span>|<span data-ttu-id="42261-136">说明</span><span class="sxs-lookup"><span data-stu-id="42261-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42261-137">id</span><span class="sxs-lookup"><span data-stu-id="42261-137">id</span></span>|<span data-ttu-id="42261-138">字符串</span><span class="sxs-lookup"><span data-stu-id="42261-138">String</span></span>|<span data-ttu-id="42261-139">API 连接器的随机生成的 ID。</span><span class="sxs-lookup"><span data-stu-id="42261-139">The randomly generated ID of the API connector.</span></span> |
|<span data-ttu-id="42261-140">displayName</span><span class="sxs-lookup"><span data-stu-id="42261-140">displayName</span></span>|<span data-ttu-id="42261-141">字符串</span><span class="sxs-lookup"><span data-stu-id="42261-141">String</span></span>| <span data-ttu-id="42261-142">API 连接器的名称。</span><span class="sxs-lookup"><span data-stu-id="42261-142">The name of the API connector.</span></span> |
|<span data-ttu-id="42261-143">targetUrl</span><span class="sxs-lookup"><span data-stu-id="42261-143">targetUrl</span></span>|<span data-ttu-id="42261-144">字符串</span><span class="sxs-lookup"><span data-stu-id="42261-144">String</span></span>| <span data-ttu-id="42261-145">要调用的 API 终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="42261-145">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="42261-146">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="42261-146">authenticationConfiguration</span></span>|[<span data-ttu-id="42261-147">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="42261-147">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="42261-148">描述用于调用 API 的身份验证配置详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="42261-148">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="42261-149">支持基本证书和 PKCS 12 客户端证书。</span><span class="sxs-lookup"><span data-stu-id="42261-149">Basic and PKCS 12 client certificate are supported.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42261-150">关系</span><span class="sxs-lookup"><span data-stu-id="42261-150">Relationships</span></span>

<span data-ttu-id="42261-151">无。</span><span class="sxs-lookup"><span data-stu-id="42261-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="42261-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42261-152">JSON representation</span></span>

<span data-ttu-id="42261-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42261-153">The following is a JSON representation of the resource.</span></span>
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
