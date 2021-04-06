---
title: apiAuthenticationConfigurationBase 资源类型
description: 表示用于调用 API 的身份验证配置的基本类型。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 915e1c0c26cee173991d75bc46a1a0230844d2ec
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507964"
---
# <a name="apiauthenticationconfigurationbase-resource-type"></a><span data-ttu-id="cfdfb-103">apiAuthenticationConfigurationBase 资源类型</span><span class="sxs-lookup"><span data-stu-id="cfdfb-103">apiAuthenticationConfigurationBase resource type</span></span>

<span data-ttu-id="cfdfb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cfdfb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cfdfb-105">用于保存用于调用 API 的身份验证信息的基类型。</span><span class="sxs-lookup"><span data-stu-id="cfdfb-105">The base type to hold authentication information for calling an API.</span></span>

<span data-ttu-id="cfdfb-106">派生类型包括：</span><span class="sxs-lookup"><span data-stu-id="cfdfb-106">Derived types include:</span></span>
- <span data-ttu-id="cfdfb-107">用于 HTTP 基本身份验证的[basicAuthentication](basicauthentication.md)</span><span class="sxs-lookup"><span data-stu-id="cfdfb-107">[basicAuthentication](basicauthentication.md) for HTTP basic authentication</span></span>
- <span data-ttu-id="cfdfb-108">[用于客户端证书身份验证的 pkcs12certificate](pkcs12certificate.md) (API 连接器创建或上载) </span><span class="sxs-lookup"><span data-stu-id="cfdfb-108">[pkcs12certificate](pkcs12certificate.md) for client certificate authentication (used for API connector create or upload)</span></span>
- <span data-ttu-id="cfdfb-109">[clientCertificateAuthentication](pkcs12certificate.md) 用于 (API 连接器客户端证书的客户端证书身份验证) </span><span class="sxs-lookup"><span data-stu-id="cfdfb-109">[clientCertificateAuthentication](pkcs12certificate.md) for client certificate authentication (used for fetching the client certificates of an API connector)</span></span>

## <a name="properties"></a><span data-ttu-id="cfdfb-110">属性</span><span class="sxs-lookup"><span data-stu-id="cfdfb-110">Properties</span></span>

|<span data-ttu-id="cfdfb-111">属性</span><span class="sxs-lookup"><span data-stu-id="cfdfb-111">Property</span></span>|<span data-ttu-id="cfdfb-112">类型</span><span class="sxs-lookup"><span data-stu-id="cfdfb-112">Type</span></span>|<span data-ttu-id="cfdfb-113">说明</span><span class="sxs-lookup"><span data-stu-id="cfdfb-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="cfdfb-114">关系</span><span class="sxs-lookup"><span data-stu-id="cfdfb-114">Relationships</span></span>

<span data-ttu-id="cfdfb-115">无。</span><span class="sxs-lookup"><span data-stu-id="cfdfb-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cfdfb-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cfdfb-116">JSON representation</span></span>

<span data-ttu-id="cfdfb-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cfdfb-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.apiAuthenticationConfigurationBase"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.apiAuthenticationConfigurationBase"
}
```
