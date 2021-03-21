---
title: authenticationMethodTarget 资源类型
description: 启用以将身份验证方法用作身份验证方法策略一部分的用户或组的集合。
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4c9265fa359e5b60da6f8e36c13d1a4340ba6d1a
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964691"
---
# <a name="authenticationmethodtarget-resource-type"></a><span data-ttu-id="4fed8-103">authenticationMethodTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="4fed8-103">authenticationMethodTarget resource type</span></span>

<span data-ttu-id="4fed8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fed8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4fed8-105">启用以将身份验证方法用作 Azure AD 中身份验证方法策略一部分的用户或组的集合。</span><span class="sxs-lookup"><span data-stu-id="4fed8-105">A collection of users or groups enabled to use an authentication method as part of an authentication method policy in Azure AD.</span></span>


## <a name="properties"></a><span data-ttu-id="4fed8-106">属性</span><span class="sxs-lookup"><span data-stu-id="4fed8-106">Properties</span></span>
|<span data-ttu-id="4fed8-107">属性</span><span class="sxs-lookup"><span data-stu-id="4fed8-107">Property</span></span>|<span data-ttu-id="4fed8-108">类型</span><span class="sxs-lookup"><span data-stu-id="4fed8-108">Type</span></span>|<span data-ttu-id="4fed8-109">说明</span><span class="sxs-lookup"><span data-stu-id="4fed8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fed8-110">id</span><span class="sxs-lookup"><span data-stu-id="4fed8-110">id</span></span>|<span data-ttu-id="4fed8-111">String</span><span class="sxs-lookup"><span data-stu-id="4fed8-111">String</span></span>|<span data-ttu-id="4fed8-112">Azure AD 用户或组的对象 ID。</span><span class="sxs-lookup"><span data-stu-id="4fed8-112">Object Id of an Azure AD user or group.</span></span>|
|<span data-ttu-id="4fed8-113">isRegistrationRequired</span><span class="sxs-lookup"><span data-stu-id="4fed8-113">isRegistrationRequired</span></span>|<span data-ttu-id="4fed8-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fed8-114">Boolean</span></span>|<span data-ttu-id="4fed8-115">确定是否强制用户注册身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="4fed8-115">Determines if the user is enforced to register the authentication method.</span></span>|
|<span data-ttu-id="4fed8-116">targetType</span><span class="sxs-lookup"><span data-stu-id="4fed8-116">targetType</span></span>|<span data-ttu-id="4fed8-117">authenticationMethodTargetType</span><span class="sxs-lookup"><span data-stu-id="4fed8-117">authenticationMethodTargetType</span></span>|<span data-ttu-id="4fed8-118">可取值为：`user`、`group`。</span><span class="sxs-lookup"><span data-stu-id="4fed8-118">Possible values are: `user`, `group`.</span></span>|
|<span data-ttu-id="4fed8-119">useForSignIn</span><span class="sxs-lookup"><span data-stu-id="4fed8-119">useForSignIn</span></span>|<span data-ttu-id="4fed8-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fed8-120">Boolean</span></span>|<span data-ttu-id="4fed8-121">确定是否可以使用身份验证方法登录到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="4fed8-121">Determines if the authentication method can be used to sign in to Azure AD.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4fed8-122">关系</span><span class="sxs-lookup"><span data-stu-id="4fed8-122">Relationships</span></span>
<span data-ttu-id="4fed8-123">无。</span><span class="sxs-lookup"><span data-stu-id="4fed8-123">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4fed8-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4fed8-124">JSON representation</span></span>
<span data-ttu-id="4fed8-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4fed8-125">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.authenticationMethodTarget",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodTarget",
  "id": "String (identifier)",
  "targetType": "String",
  "isRegistrationRequired": "Boolean",
  "useForSignIn": "Boolean"
}
```
