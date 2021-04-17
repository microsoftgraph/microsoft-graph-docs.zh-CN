---
title: userFlowApiConnectorConfiguration 资源类型
description: 表示为用户流启用的 API 连接器。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b9d9b87bf59a796e8c79875a8506fccdd4d3447b
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882943"
---
# <a name="userflowapiconnectorconfiguration-resource-type"></a><span data-ttu-id="ed72a-103">userFlowApiConnectorConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="ed72a-103">userFlowApiConnectorConfiguration resource type</span></span>

<span data-ttu-id="ed72a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed72a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed72a-105">定义在用户流中的特定点调用的 API。</span><span class="sxs-lookup"><span data-stu-id="ed72a-105">Defines the APIs that are called at specific points in the user flow.</span></span>  <span data-ttu-id="ed72a-106">此对象的每个关系对应于可配置为调用 API 连接器的用户流中的特定步骤。</span><span class="sxs-lookup"><span data-stu-id="ed72a-106">Each relationship of this object corresponds to a specific step in the user flow that can be configured to call an API connector.</span></span>

## <a name="relationships"></a><span data-ttu-id="ed72a-107">关系</span><span class="sxs-lookup"><span data-stu-id="ed72a-107">Relationships</span></span>

| <span data-ttu-id="ed72a-108">关系</span><span class="sxs-lookup"><span data-stu-id="ed72a-108">Relationship</span></span>            | <span data-ttu-id="ed72a-109">类型</span><span class="sxs-lookup"><span data-stu-id="ed72a-109">Type</span></span>                                            | <span data-ttu-id="ed72a-110">说明</span><span class="sxs-lookup"><span data-stu-id="ed72a-110">Description</span></span>                                                                                                                                             |
| :---------------------- | :---------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="ed72a-111">postFederationSignup</span><span class="sxs-lookup"><span data-stu-id="ed72a-111">postFederationSignup</span></span>    | [<span data-ttu-id="ed72a-112">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="ed72a-112">identityApiConnector</span></span>](identityapiconnector.md) | <span data-ttu-id="ed72a-113">指定与外部标识提供程序建立联盟后要调用的 API。</span><span class="sxs-lookup"><span data-stu-id="ed72a-113">Specifies an API to call after federation with an external identity provider.</span></span> <span data-ttu-id="ed72a-114">例如，当用户注册 Google、Facebook 或 Azure AD API 时， (不适用于登录帐户) 。</span><span class="sxs-lookup"><span data-stu-id="ed72a-114">For example, a Google, Facebook, or Azure AD API is completed when the user is signing up (does not apply to sign-in).</span></span> |
| <span data-ttu-id="ed72a-115">postAttributeCollection</span><span class="sxs-lookup"><span data-stu-id="ed72a-115">postAttributeCollection</span></span> | [<span data-ttu-id="ed72a-116">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="ed72a-116">identityApiConnector</span></span>](identityapiconnector.md) | <span data-ttu-id="ed72a-117">指定在用户提交收集的属性后以及注册期间创建用户帐户之前要调用的 API。</span><span class="sxs-lookup"><span data-stu-id="ed72a-117">Specifies an API to call after a user submits the collected attributes and before the user account is created during sign-up.</span></span>                                                      |

## <a name="json-representation"></a><span data-ttu-id="ed72a-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ed72a-118">JSON representation</span></span>

<span data-ttu-id="ed72a-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ed72a-119">The following is a JSON representation of the resource.</span></span>
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
