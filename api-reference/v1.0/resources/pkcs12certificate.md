---
title: pkcs12Certificate 资源类型
description: 表示用于上载 pkcs12Certificate 的配置。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 60350908901293ec9bf090c9e2bc174d70c922e5
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882394"
---
# <a name="pkcs12certificate-resource-type"></a><span data-ttu-id="61500-103">pkcs12Certificate 资源类型</span><span class="sxs-lookup"><span data-stu-id="61500-103">pkcs12Certificate resource type</span></span>

<span data-ttu-id="61500-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="61500-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="61500-105">表示在使用 HTTPS 客户端证书身份验证调用 API 连接器终结点时用于上载证书的配置。</span><span class="sxs-lookup"><span data-stu-id="61500-105">Represents the configuration used to upload a certificate when using HTTPS client-certificate authentication for calling an API connector endpoint.</span></span> <span data-ttu-id="61500-106">客户端证书身份验证是基于相互证书的身份验证，其中客户端向 API 终结点提供客户端证书以证明其身份。</span><span class="sxs-lookup"><span data-stu-id="61500-106">Client certificate authentication is a mutual certificate-based authentication, where the client provides a client certificate to an API endpoint to prove its identity.</span></span> <span data-ttu-id="61500-107">Azure AD 将 API 连接器的配置证书发送到给定的 API 终结点，然后验证该证书。</span><span class="sxs-lookup"><span data-stu-id="61500-107">The configured certificate of an API connector is sent by Azure AD to the given API endpoint, which then validates the certificate.</span></span>

<span data-ttu-id="61500-108">继承自 [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="61500-108">Inherits from [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="61500-109">属性</span><span class="sxs-lookup"><span data-stu-id="61500-109">Properties</span></span>

|<span data-ttu-id="61500-110">属性</span><span class="sxs-lookup"><span data-stu-id="61500-110">Property</span></span>|<span data-ttu-id="61500-111">类型</span><span class="sxs-lookup"><span data-stu-id="61500-111">Type</span></span>|<span data-ttu-id="61500-112">说明</span><span class="sxs-lookup"><span data-stu-id="61500-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61500-113">pkcs12Value</span><span class="sxs-lookup"><span data-stu-id="61500-113">pkcs12Value</span></span>|<span data-ttu-id="61500-114">String</span><span class="sxs-lookup"><span data-stu-id="61500-114">String</span></span>| <span data-ttu-id="61500-115">表示发送的 pfx 内容。</span><span class="sxs-lookup"><span data-stu-id="61500-115">Represents the pfx content that is sent.</span></span> <span data-ttu-id="61500-116">该值应为实际证书内容的 Base64 编码版本。</span><span class="sxs-lookup"><span data-stu-id="61500-116">The value should be a base-64 encoded version of the actual certificate content.</span></span> <span data-ttu-id="61500-117">必填。</span><span class="sxs-lookup"><span data-stu-id="61500-117">Required.</span></span>|
|<span data-ttu-id="61500-118">密码</span><span class="sxs-lookup"><span data-stu-id="61500-118">password</span></span>|<span data-ttu-id="61500-119">String</span><span class="sxs-lookup"><span data-stu-id="61500-119">String</span></span>| <span data-ttu-id="61500-120">pfx 文件的密码。</span><span class="sxs-lookup"><span data-stu-id="61500-120">The password for the pfx file.</span></span> <span data-ttu-id="61500-121">必填。</span><span class="sxs-lookup"><span data-stu-id="61500-121">Required.</span></span> <span data-ttu-id="61500-122">如果未使用密码，则仍必须提供 的值 `""` 。</span><span class="sxs-lookup"><span data-stu-id="61500-122">If no password is used, you must still provide a value of `""`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="61500-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="61500-123">JSON representation</span></span>

<span data-ttu-id="61500-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="61500-124">The following is a JSON representation of the resource.</span></span>
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
