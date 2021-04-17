---
title: identityApiConnector 资源类型
description: 表示 Azure Active Directory 租户中的 API 连接器。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 8fc0ff1915bd76a35d9eb0c0041e1628fde41981
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882825"
---
# <a name="identityapiconnector-resource-type"></a><span data-ttu-id="4502f-103">identityApiConnector 资源类型</span><span class="sxs-lookup"><span data-stu-id="4502f-103">identityApiConnector resource type</span></span>

<span data-ttu-id="4502f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4502f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4502f-105">表示 Azure Active Directory 中的 API 连接器 (Azure AD) 租户。</span><span class="sxs-lookup"><span data-stu-id="4502f-105">Represents API connectors in an Azure Active Directory (Azure AD) tenants.</span></span>

<span data-ttu-id="4502f-106">Azure AD 外部标识自助注册用户流中使用的 API 连接器允许你在执行用户流期间调用 API。</span><span class="sxs-lookup"><span data-stu-id="4502f-106">An API connector used in your Azure AD External Identities self-service sign-up user flows allows you to call an API during the execution of the user flow.</span></span> <span data-ttu-id="4502f-107">API 连接器提供调用 API 时需要的信息，包括终结点 URL 和身份验证。</span><span class="sxs-lookup"><span data-stu-id="4502f-107">An API connector provides the information needed to call an API including an endpoint URL and authentication.</span></span> <span data-ttu-id="4502f-108">API 连接器可在用户流中的特定步骤使用，以影响用户流的执行。</span><span class="sxs-lookup"><span data-stu-id="4502f-108">An API connector can be used at a specific step in a user flow to affect the execution of the user flow.</span></span> <span data-ttu-id="4502f-109">例如，API 响应可以阻止用户注册、显示输入验证错误或覆盖用户收集的属性。</span><span class="sxs-lookup"><span data-stu-id="4502f-109">For example, the API response can block a user from signing up, show an input validation error, or overwrite user collected attributes.</span></span>

<span data-ttu-id="4502f-110">使用 [b2xIdentityUserFlow](b2xidentityuserflow.md) API 从外部标识自助注册用户流使用 API 连接器。</span><span class="sxs-lookup"><span data-stu-id="4502f-110">Use the [b2xIdentityUserFlow](b2xidentityuserflow.md) API to use an API connector from an External Identities self-service sign-up user flow.</span></span>

## <a name="methods"></a><span data-ttu-id="4502f-111">方法</span><span class="sxs-lookup"><span data-stu-id="4502f-111">Methods</span></span>

|<span data-ttu-id="4502f-112">方法</span><span class="sxs-lookup"><span data-stu-id="4502f-112">Method</span></span>|<span data-ttu-id="4502f-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="4502f-113">Return type</span></span>|<span data-ttu-id="4502f-114">Description</span><span class="sxs-lookup"><span data-stu-id="4502f-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4502f-115">List</span><span class="sxs-lookup"><span data-stu-id="4502f-115">List</span></span>](../api/identityapiconnector-list.md)|<span data-ttu-id="4502f-116">[identityApiConnector](../resources/identityapiconnector.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4502f-116">[identityApiConnector](../resources/identityapiconnector.md) collection</span></span>| <span data-ttu-id="4502f-117">获取 API 连接器列表</span><span class="sxs-lookup"><span data-stu-id="4502f-117">Get a list of API connectors</span></span>|
|[<span data-ttu-id="4502f-118">Create</span><span class="sxs-lookup"><span data-stu-id="4502f-118">Create</span></span>](../api/identityapiconnector-create.md)|[<span data-ttu-id="4502f-119">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="4502f-119">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="4502f-120">创建新的 API 连接器。</span><span class="sxs-lookup"><span data-stu-id="4502f-120">Create a new API connector.</span></span> |
|[<span data-ttu-id="4502f-121">Get</span><span class="sxs-lookup"><span data-stu-id="4502f-121">Get</span></span>](../api/identityapiconnector-get.md)|[<span data-ttu-id="4502f-122">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="4502f-122">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="4502f-123">读取 [identityApiConnector 对象](../resources/identityapiconnector.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="4502f-123">Read the properties of an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>|
|[<span data-ttu-id="4502f-124">更新</span><span class="sxs-lookup"><span data-stu-id="4502f-124">Update</span></span>](../api/identityapiconnector-update.md)|[<span data-ttu-id="4502f-125">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="4502f-125">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="4502f-126">更新 API 连接器的属性。</span><span class="sxs-lookup"><span data-stu-id="4502f-126">Update the properties of an API connector.</span></span>|
|[<span data-ttu-id="4502f-127">上载客户端证书</span><span class="sxs-lookup"><span data-stu-id="4502f-127">Upload client certificate</span></span>](../api/identityapiconnector-uploadclientcertificate.md)|[<span data-ttu-id="4502f-128">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="4502f-128">identityApiConnector</span></span>](identityapiconnector.md)|<span data-ttu-id="4502f-129">上载客户端证书以用于身份验证。</span><span class="sxs-lookup"><span data-stu-id="4502f-129">Upload a client certificate to use for authentication.</span></span>|
|[<span data-ttu-id="4502f-130">删除</span><span class="sxs-lookup"><span data-stu-id="4502f-130">Delete</span></span>](../api/identityapiconnector-delete.md)|<span data-ttu-id="4502f-131">无</span><span class="sxs-lookup"><span data-stu-id="4502f-131">None</span></span>|<span data-ttu-id="4502f-132">删除 API 连接器。</span><span class="sxs-lookup"><span data-stu-id="4502f-132">Delete an API connector.</span></span>|

## <a name="properties"></a><span data-ttu-id="4502f-133">属性</span><span class="sxs-lookup"><span data-stu-id="4502f-133">Properties</span></span>

|<span data-ttu-id="4502f-134">属性</span><span class="sxs-lookup"><span data-stu-id="4502f-134">Property</span></span>|<span data-ttu-id="4502f-135">类型</span><span class="sxs-lookup"><span data-stu-id="4502f-135">Type</span></span>|<span data-ttu-id="4502f-136">说明</span><span class="sxs-lookup"><span data-stu-id="4502f-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4502f-137">id</span><span class="sxs-lookup"><span data-stu-id="4502f-137">id</span></span>|<span data-ttu-id="4502f-138">String</span><span class="sxs-lookup"><span data-stu-id="4502f-138">String</span></span>|<span data-ttu-id="4502f-139">API 连接器的随机生成的标识符。</span><span class="sxs-lookup"><span data-stu-id="4502f-139">The randomly generated identifier of the API connector.</span></span> |
|<span data-ttu-id="4502f-140">displayName</span><span class="sxs-lookup"><span data-stu-id="4502f-140">displayName</span></span>|<span data-ttu-id="4502f-141">String</span><span class="sxs-lookup"><span data-stu-id="4502f-141">String</span></span>| <span data-ttu-id="4502f-142">API 连接器的名称。</span><span class="sxs-lookup"><span data-stu-id="4502f-142">The name of the API connector.</span></span> |
|<span data-ttu-id="4502f-143">targetUrl</span><span class="sxs-lookup"><span data-stu-id="4502f-143">targetUrl</span></span>|<span data-ttu-id="4502f-144">String</span><span class="sxs-lookup"><span data-stu-id="4502f-144">String</span></span>| <span data-ttu-id="4502f-145">要调用的 API 终结点的 URL。</span><span class="sxs-lookup"><span data-stu-id="4502f-145">The URL of the API endpoint to call.</span></span> |
|<span data-ttu-id="4502f-146">authenticationConfiguration</span><span class="sxs-lookup"><span data-stu-id="4502f-146">authenticationConfiguration</span></span>|[<span data-ttu-id="4502f-147">apiAuthenticationConfigurationBase</span><span class="sxs-lookup"><span data-stu-id="4502f-147">apiAuthenticationConfigurationBase</span></span>](../resources/apiauthenticationconfigurationbase.md)|<span data-ttu-id="4502f-148">描述用于调用 API 的身份验证配置详细信息的对象。</span><span class="sxs-lookup"><span data-stu-id="4502f-148">The object which describes the authentication configuration details for calling the API.</span></span> <span data-ttu-id="4502f-149">支持基本证书和 PKCS 12 客户端证书。</span><span class="sxs-lookup"><span data-stu-id="4502f-149">Basic and PKCS 12 client certificate are supported.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4502f-150">关系</span><span class="sxs-lookup"><span data-stu-id="4502f-150">Relationships</span></span>

<span data-ttu-id="4502f-151">无。</span><span class="sxs-lookup"><span data-stu-id="4502f-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4502f-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4502f-152">JSON representation</span></span>

<span data-ttu-id="4502f-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4502f-153">The following is a JSON representation of the resource.</span></span>
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
