---
title: pkcs12Certificate 资源类型
description: 表示在 API 调用中上传 pkcs12Certificate 的配置。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f312a7be0bd29d57c1a6b7dc5c7e5d72e6d41206
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509373"
---
# <a name="pkcs12certificate-resource-type"></a><span data-ttu-id="dbd75-103">pkcs12Certificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="dbd75-103">pkcs12Certificate resource type</span></span>

<span data-ttu-id="dbd75-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbd75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dbd75-105">表示在使用 HTTPS **客户端** 证书身份验证调用 API 连接器终结点时用于上载证书的配置。</span><span class="sxs-lookup"><span data-stu-id="dbd75-105">Represents the configuration used to **upload** a certificate when using HTTPS client-certificate authentication for calling an API connector endpoint.</span></span> <span data-ttu-id="dbd75-106">客户端证书身份验证是基于相互证书的身份验证，其中客户端向 API 终结点提供客户端证书以证明其身份。</span><span class="sxs-lookup"><span data-stu-id="dbd75-106">Client certificate authentication is a mutual certificate-based authentication, where the client provides a client certificate to an API endpoint to prove its identity.</span></span> <span data-ttu-id="dbd75-107">Azure AD 将 API 连接器的配置证书发送到给定的 API 终结点，然后验证该证书。</span><span class="sxs-lookup"><span data-stu-id="dbd75-107">The configured certificate of an API connector is sent by Azure AD to the given API endpoint, which then validates the certificate.</span></span>

<span data-ttu-id="dbd75-108">继承自 [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="dbd75-108">Inherits from [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dbd75-109">属性</span><span class="sxs-lookup"><span data-stu-id="dbd75-109">Properties</span></span>

|<span data-ttu-id="dbd75-110">属性</span><span class="sxs-lookup"><span data-stu-id="dbd75-110">Property</span></span>|<span data-ttu-id="dbd75-111">类型</span><span class="sxs-lookup"><span data-stu-id="dbd75-111">Type</span></span>|<span data-ttu-id="dbd75-112">说明</span><span class="sxs-lookup"><span data-stu-id="dbd75-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbd75-113">pkcs12Value</span><span class="sxs-lookup"><span data-stu-id="dbd75-113">pkcs12Value</span></span>|<span data-ttu-id="dbd75-114">字符串</span><span class="sxs-lookup"><span data-stu-id="dbd75-114">String</span></span>| <span data-ttu-id="dbd75-115">这是用于发送 pfx 内容的字段。</span><span class="sxs-lookup"><span data-stu-id="dbd75-115">This is the field for sending pfx content.</span></span> <span data-ttu-id="dbd75-116">该值应为实际证书内容的 Base64 编码版本。</span><span class="sxs-lookup"><span data-stu-id="dbd75-116">The value should be a base-64 encoded version of the actual certificate content.</span></span> <span data-ttu-id="dbd75-117">必填。</span><span class="sxs-lookup"><span data-stu-id="dbd75-117">Required.</span></span>|
|<span data-ttu-id="dbd75-118">密码</span><span class="sxs-lookup"><span data-stu-id="dbd75-118">password</span></span>|<span data-ttu-id="dbd75-119">String</span><span class="sxs-lookup"><span data-stu-id="dbd75-119">String</span></span>| <span data-ttu-id="dbd75-120">这是 pfx 文件的密码。</span><span class="sxs-lookup"><span data-stu-id="dbd75-120">This is the password for the pfx file.</span></span> <span data-ttu-id="dbd75-121">必填。</span><span class="sxs-lookup"><span data-stu-id="dbd75-121">Required.</span></span> <span data-ttu-id="dbd75-122">如果未使用密码，则仍必须提供 的值 `""` 。</span><span class="sxs-lookup"><span data-stu-id="dbd75-122">If no password is used, must still provide a value of `""`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dbd75-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dbd75-123">JSON representation</span></span>

<span data-ttu-id="dbd75-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dbd75-124">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.pkcs12Certificate"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.pkcs12Certificate",
  "pkcs12Value": "String",
  "password": "String"
}
```
