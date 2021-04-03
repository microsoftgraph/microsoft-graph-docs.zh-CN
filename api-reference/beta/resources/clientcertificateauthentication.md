---
title: clientCertificateAuthentication 资源类型
description: 表示用于获取 API 调用中的 clientCertificateAuthentication 的配置。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0e88a1de011fb975afae49d53b8707b95e16157c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509391"
---
# <a name="clientcertificateauthentication-resource-type"></a><span data-ttu-id="d4787-103">clientCertificateAuthentication 资源类型</span><span class="sxs-lookup"><span data-stu-id="d4787-103">clientCertificateAuthentication resource type</span></span>

<span data-ttu-id="d4787-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4787-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4787-105">派生自 apiAuthenticationConfigurationBase 的类型，用于表示基于 Pkcs12 的客户端证书身份验证。</span><span class="sxs-lookup"><span data-stu-id="d4787-105">A type derived from apiAuthenticationConfigurationBase which is used to represent Pkcs12 based client certificate authentication.</span></span> <span data-ttu-id="d4787-106">这用于检索上载的证书的公共属性。</span><span class="sxs-lookup"><span data-stu-id="d4787-106">This is used to retrieve the public properties of uploaded certificates.</span></span>

<span data-ttu-id="d4787-107">继承自 [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="d4787-107">Inherits from [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d4787-108">属性</span><span class="sxs-lookup"><span data-stu-id="d4787-108">Properties</span></span>

|<span data-ttu-id="d4787-109">属性</span><span class="sxs-lookup"><span data-stu-id="d4787-109">Property</span></span>|<span data-ttu-id="d4787-110">类型</span><span class="sxs-lookup"><span data-stu-id="d4787-110">Type</span></span>|<span data-ttu-id="d4787-111">说明</span><span class="sxs-lookup"><span data-stu-id="d4787-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4787-112">certificateList</span><span class="sxs-lookup"><span data-stu-id="d4787-112">certificateList</span></span>| <span data-ttu-id="d4787-113">[pkcs12CertificateInformation](../resources/pkcs12CertificateInformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d4787-113">[pkcs12CertificateInformation](../resources/pkcs12CertificateInformation.md) collection</span></span>| <span data-ttu-id="d4787-114">为此 API 连接器上载的证书列表。</span><span class="sxs-lookup"><span data-stu-id="d4787-114">The list of certificates uploaded for this API connector.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4787-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d4787-115">JSON representation</span></span>

<span data-ttu-id="d4787-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d4787-116">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.clientCertificateAuthentication"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.clientCertificateAuthentication",
  "certificateList": "Collection(microsoft.graph.pkcs12CertificateInformation)",
}
```
