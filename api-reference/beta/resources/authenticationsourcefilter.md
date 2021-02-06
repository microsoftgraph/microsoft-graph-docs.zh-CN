---
title: authenticationSourceFilter 资源类型
description: 基于用于确定是否执行侦听器的身份验证源进行筛选。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 4736be415faab65c6ce3b572a1273a73c707ee43
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128629"
---
# <a name="authenticationsourcefilter-resource-type"></a><span data-ttu-id="c92c2-103">authenticationSourceFilter 资源类型</span><span class="sxs-lookup"><span data-stu-id="c92c2-103">authenticationSourceFilter resource type</span></span>

<span data-ttu-id="c92c2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c92c2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c92c2-105">基于用于确定是否评估侦听器的身份验证源进行筛选。</span><span class="sxs-lookup"><span data-stu-id="c92c2-105">Filter based on the source of the authentication that is used to determine whether the listener is evaluated.</span></span>

<span data-ttu-id="c92c2-106">**includeApplications** 属性可用于在 Azure Active Directory 中启用应用程序的自助注册。</span><span class="sxs-lookup"><span data-stu-id="c92c2-106">The **includeApplications** property can be used to enable self-service sign up on an application in Azure Active Directory.</span></span> <span data-ttu-id="c92c2-107">阅读我们的文档以在自助服务注册用户流中启用 [应用程序，了解更多信息](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow#add-applications-to-the-self-service-sign-up-user-flow)。</span><span class="sxs-lookup"><span data-stu-id="c92c2-107">Learn more by reading our documentation for [enabling applications in a self-service sign up user flow](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow#add-applications-to-the-self-service-sign-up-user-flow).</span></span>

## <a name="properties"></a><span data-ttu-id="c92c2-108">属性</span><span class="sxs-lookup"><span data-stu-id="c92c2-108">Properties</span></span>

|<span data-ttu-id="c92c2-109">属性</span><span class="sxs-lookup"><span data-stu-id="c92c2-109">Property</span></span>|<span data-ttu-id="c92c2-110">类型</span><span class="sxs-lookup"><span data-stu-id="c92c2-110">Type</span></span>|<span data-ttu-id="c92c2-111">说明</span><span class="sxs-lookup"><span data-stu-id="c92c2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c92c2-112">includeApplications</span><span class="sxs-lookup"><span data-stu-id="c92c2-112">includeApplications</span></span>|<span data-ttu-id="c92c2-113">字符串集合</span><span class="sxs-lookup"><span data-stu-id="c92c2-113">String collection</span></span>|<span data-ttu-id="c92c2-114">要包含用于评估 [authenticationListener 的应用程序](../resources/authenticationlistener.md)。</span><span class="sxs-lookup"><span data-stu-id="c92c2-114">Applications to include for evaluation of the [authenticationListener](../resources/authenticationlistener.md).</span></span> <span data-ttu-id="c92c2-115">当在身份验证流中用作客户端应用程序时，这些应用程序将触发关联的操作。</span><span class="sxs-lookup"><span data-stu-id="c92c2-115">These applications trigger the associated action when used as the client application in the authentication flow.</span></span> <span data-ttu-id="c92c2-116">应用程序标识是应用程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="c92c2-116">The application identifer is the application's client id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c92c2-117">关系</span><span class="sxs-lookup"><span data-stu-id="c92c2-117">Relationships</span></span>

<span data-ttu-id="c92c2-118">无。</span><span class="sxs-lookup"><span data-stu-id="c92c2-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c92c2-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c92c2-119">JSON representation</span></span>

<span data-ttu-id="c92c2-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c92c2-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationSourceFilter"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.authenticationSourceFilter",
  "includeApplications": [
    "String"
  ]
}
```
