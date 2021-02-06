---
title: userFlowApiConnectorConfiguration 资源类型
description: 表示为用户流启用的 API 连接器。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 9f8e9732759a609eabb6733629a97c82afaba364
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132977"
---
# <a name="userflowapiconnectorconfiguration-resource-type"></a><span data-ttu-id="f325c-103">userFlowApiConnectorConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="f325c-103">userFlowApiConnectorConfiguration resource type</span></span>

<span data-ttu-id="f325c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f325c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f325c-105">定义在用户流中的特定点调用哪些 API。</span><span class="sxs-lookup"><span data-stu-id="f325c-105">Defines which APIs are called at specific points in the user flow.</span></span>  <span data-ttu-id="f325c-106">此对象的每个关系对应于可配置为调用 API 连接器的用户流中的特定步骤。</span><span class="sxs-lookup"><span data-stu-id="f325c-106">Each relationship of this object corresponds to a specific step in the user flow that can be configured to call an API connector.</span></span>

## <a name="relationships"></a><span data-ttu-id="f325c-107">关系</span><span class="sxs-lookup"><span data-stu-id="f325c-107">Relationships</span></span>

| <span data-ttu-id="f325c-108">关系</span><span class="sxs-lookup"><span data-stu-id="f325c-108">Relationship</span></span>            | <span data-ttu-id="f325c-109">类型</span><span class="sxs-lookup"><span data-stu-id="f325c-109">Type</span></span>                                            | <span data-ttu-id="f325c-110">说明</span><span class="sxs-lookup"><span data-stu-id="f325c-110">Description</span></span>                                                                                                                                             |
| :---------------------- | :---------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="f325c-111">postFederationSignup</span><span class="sxs-lookup"><span data-stu-id="f325c-111">postFederationSignup</span></span>    | [<span data-ttu-id="f325c-112">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="f325c-112">identityApiConnector</span></span>](identityapiconnector.md) | <span data-ttu-id="f325c-113">指定在用户注册时与外部标识提供程序 (如 Google、Facebook 或 Azure AD) 的联盟完成后要调用的 API (不适用于登录) 。</span><span class="sxs-lookup"><span data-stu-id="f325c-113">Specifies an API to call after federation with an external identity provider (like Google, Facebook, or Azure AD) is completed when user is signing up (does not apply to sign in).</span></span> |
| <span data-ttu-id="f325c-114">postAttributeCollection</span><span class="sxs-lookup"><span data-stu-id="f325c-114">postAttributeCollection</span></span> | [<span data-ttu-id="f325c-115">identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="f325c-115">identityApiConnector</span></span>](identityapiconnector.md) | <span data-ttu-id="f325c-116">指定在用户提交收集的属性后以及注册期间创建用户之前要调用的 API。</span><span class="sxs-lookup"><span data-stu-id="f325c-116">Specifies an API to call after a user submits collected attributes and before the user is created during sign up.</span></span>                                                      |

## <a name="json-representation"></a><span data-ttu-id="f325c-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f325c-117">JSON representation</span></span>

<span data-ttu-id="f325c-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f325c-118">The following is a JSON representation of the resource.</span></span>
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
    "Error: Resource userFlowApiConnectorConfiguration has documented navigation properties, but we thought it was a complex type!"
  ]
}-->
