---
title: userFlowApiConnectorConfiguration 资源类型
description: 表示为用户流启用的 API 连接器。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 78e93f4b743f57a68faad530f2a26ad6dead8a08
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292884"
---
# <a name="userflowapiconnectorconfiguration-resource-type"></a><span data-ttu-id="4327b-103">userFlowApiConnectorConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="4327b-103">userFlowApiConnectorConfiguration resource type</span></span>

<span data-ttu-id="4327b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4327b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4327b-105">定义在用户流中的特定点调用哪些 API。</span><span class="sxs-lookup"><span data-stu-id="4327b-105">Defines which APIs are called at specific points in the user flow.</span></span>  <span data-ttu-id="4327b-106">此对象的每个关系对应于用户流中可配置为调用 API 连接器的特定步骤。</span><span class="sxs-lookup"><span data-stu-id="4327b-106">Each relationship of this object corresponds to a specific step in the user flow that can be configured to call an API connector.</span></span>

## <a name="relationships"></a><span data-ttu-id="4327b-107">关系</span><span class="sxs-lookup"><span data-stu-id="4327b-107">Relationships</span></span>

| <span data-ttu-id="4327b-108">关系</span><span class="sxs-lookup"><span data-stu-id="4327b-108">Relationship</span></span>            | <span data-ttu-id="4327b-109">类型</span><span class="sxs-lookup"><span data-stu-id="4327b-109">Type</span></span>                                            | <span data-ttu-id="4327b-110">说明</span><span class="sxs-lookup"><span data-stu-id="4327b-110">Description</span></span>                                                                                                                                             |
| :---------------------- | :---------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="4327b-111">postFederationSignup</span><span class="sxs-lookup"><span data-stu-id="4327b-111">postFederationSignup</span></span>    | [<span data-ttu-id="4327b-112">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="4327b-112">identityApiConnector</span></span>](identityapiconnector.md) | <span data-ttu-id="4327b-113">指定在用户注册 (时完成与外部标识提供程序 (如 Google、Facebook 或 Azure AD) 的联盟后要调用的 API (不适用于登录) 。</span><span class="sxs-lookup"><span data-stu-id="4327b-113">Specifies an API to call after federation with an external identity provider (like Google, Facebook, or Azure AD) is completed when user is signing up (does not apply to sign in).</span></span> |
| <span data-ttu-id="4327b-114">postAttributeCollection</span><span class="sxs-lookup"><span data-stu-id="4327b-114">postAttributeCollection</span></span> | [<span data-ttu-id="4327b-115">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="4327b-115">identityApiConnector</span></span>](identityapiconnector.md) | <span data-ttu-id="4327b-116">指定在用户提交收集的属性后以及注册期间创建用户之前要调用的 API。</span><span class="sxs-lookup"><span data-stu-id="4327b-116">Specifies an API to call after a user submits collected attributes and before the user is created during sign up.</span></span>                                                      |

## <a name="json-representation"></a><span data-ttu-id="4327b-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4327b-117">JSON representation</span></span>

<span data-ttu-id="4327b-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4327b-118">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userFlowApiConnectorConfiguration"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowApiConnectorConfiguration"
}
```

<!-- {
  "type": "#page.annotation",
  "description": "User flow API Connector Configuration",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
