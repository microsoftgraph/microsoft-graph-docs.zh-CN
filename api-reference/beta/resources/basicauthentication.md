---
title: basicAuthentication 资源类型
description: 表示在 API 调用中使用基本身份验证的配置。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9de5fad9746e8562f51d1ddc8fcea350c41979ed
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720154"
---
# <a name="basicauthentication-resource-type"></a><span data-ttu-id="11ac4-103">basicAuthentication 资源类型</span><span class="sxs-lookup"><span data-stu-id="11ac4-103">basicAuthentication resource type</span></span>

<span data-ttu-id="11ac4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11ac4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11ac4-105">表示在 API 调用中使用 HTTP 基本身份验证的配置，这需要用户名和密码。</span><span class="sxs-lookup"><span data-stu-id="11ac4-105">Represents configuration for using HTTP Basic authentication, which entails a username and password, in an API call.</span></span> <span data-ttu-id="11ac4-106">用户名和密码作为授权标头发送，就像用户名：password 的 `Basic {value}` `value` base 64 编码版本一样。</span><span class="sxs-lookup"><span data-stu-id="11ac4-106">The username and password is sent as the Authorization header as `Basic {value}` where `value` is base 64 encoded version of username:password.</span></span>

<span data-ttu-id="11ac4-107">继承自 [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md)。</span><span class="sxs-lookup"><span data-stu-id="11ac4-107">Inherits from [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="11ac4-108">属性</span><span class="sxs-lookup"><span data-stu-id="11ac4-108">Properties</span></span>

|<span data-ttu-id="11ac4-109">属性</span><span class="sxs-lookup"><span data-stu-id="11ac4-109">Property</span></span>|<span data-ttu-id="11ac4-110">类型</span><span class="sxs-lookup"><span data-stu-id="11ac4-110">Type</span></span>|<span data-ttu-id="11ac4-111">说明</span><span class="sxs-lookup"><span data-stu-id="11ac4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11ac4-112">username</span><span class="sxs-lookup"><span data-stu-id="11ac4-112">username</span></span>|<span data-ttu-id="11ac4-113">String</span><span class="sxs-lookup"><span data-stu-id="11ac4-113">String</span></span>| <span data-ttu-id="11ac4-114">用户名。</span><span class="sxs-lookup"><span data-stu-id="11ac4-114">The username.</span></span> |
|<span data-ttu-id="11ac4-115">密码</span><span class="sxs-lookup"><span data-stu-id="11ac4-115">password</span></span>|<span data-ttu-id="11ac4-116">String</span><span class="sxs-lookup"><span data-stu-id="11ac4-116">String</span></span>| <span data-ttu-id="11ac4-117">密码。</span><span class="sxs-lookup"><span data-stu-id="11ac4-117">The password.</span></span> <span data-ttu-id="11ac4-118">响应中不会返回它。</span><span class="sxs-lookup"><span data-stu-id="11ac4-118">It is not returned in the responses.</span></span> |

## <a name="relationships"></a><span data-ttu-id="11ac4-119">关系</span><span class="sxs-lookup"><span data-stu-id="11ac4-119">Relationships</span></span>

<span data-ttu-id="11ac4-120">无。</span><span class="sxs-lookup"><span data-stu-id="11ac4-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="11ac4-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11ac4-121">JSON representation</span></span>

<span data-ttu-id="11ac4-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11ac4-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.basicAuthentication"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.basicAuthentication",
  "password": "String",
  "username": "String"
}
```
