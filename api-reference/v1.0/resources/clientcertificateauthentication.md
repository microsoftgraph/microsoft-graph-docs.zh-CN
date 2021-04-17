---
title: clientCertificateAuthentication 资源类型
description: 表示用于检索 clientCertificateAuthentication 的配置。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 69870b1160078495d3b9440260aab1f231041eef
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882428"
---
# <a name="clientcertificateauthentication-resource-type"></a><span data-ttu-id="bac4c-103">clientCertificateAuthentication 资源类型</span><span class="sxs-lookup"><span data-stu-id="bac4c-103">clientCertificateAuthentication resource type</span></span>

<span data-ttu-id="bac4c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bac4c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bac4c-105">派生自 apiAuthenticationConfigurationBase 的类型，用于表示基于 Pkcs12 的客户端证书身份验证。</span><span class="sxs-lookup"><span data-stu-id="bac4c-105">A type derived from apiAuthenticationConfigurationBase that is used to represent a Pkcs12-based client certificate authentication.</span></span> <span data-ttu-id="bac4c-106">这用于检索上载的证书的公共属性。</span><span class="sxs-lookup"><span data-stu-id="bac4c-106">This is used to retrieve the public properties of uploaded certificates.</span></span>

<span data-ttu-id="bac4c-107">继承自 [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="bac4c-107">Inherits from [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bac4c-108">属性</span><span class="sxs-lookup"><span data-stu-id="bac4c-108">Properties</span></span>

|<span data-ttu-id="bac4c-109">属性</span><span class="sxs-lookup"><span data-stu-id="bac4c-109">Property</span></span>|<span data-ttu-id="bac4c-110">类型</span><span class="sxs-lookup"><span data-stu-id="bac4c-110">Type</span></span>|<span data-ttu-id="bac4c-111">说明</span><span class="sxs-lookup"><span data-stu-id="bac4c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bac4c-112">certificateList</span><span class="sxs-lookup"><span data-stu-id="bac4c-112">certificateList</span></span>| <span data-ttu-id="bac4c-113">[pkcs12CertificateInformation](../resources/pkcs12CertificateInformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="bac4c-113">[pkcs12CertificateInformation](../resources/pkcs12CertificateInformation.md) collection</span></span>| <span data-ttu-id="bac4c-114">为此 API 连接器上载的证书列表。</span><span class="sxs-lookup"><span data-stu-id="bac4c-114">The list of certificates uploaded for this API connector.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bac4c-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bac4c-115">JSON representation</span></span>

<span data-ttu-id="bac4c-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bac4c-116">The following is a JSON representation of the resource.</span></span>
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
