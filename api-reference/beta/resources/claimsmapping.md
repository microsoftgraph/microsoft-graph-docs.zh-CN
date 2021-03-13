---
title: claimsMapping 资源类型
description: 从令牌中的将声明映射到 Azure Active Directory B2C 可识别和使用的声明。
author: namkedia
localization_priority: Priority
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1863c6bf6f28e0e8ae8a3d1133330337a7420c0a
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761840"
---
# <a name="claimsmapping-resource-type"></a><span data-ttu-id="d62f4-103">claimsMapping 资源类型</span><span class="sxs-lookup"><span data-stu-id="d62f4-103">claimsMapping resource type</span></span>

<span data-ttu-id="d62f4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d62f4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d62f4-105">自定义标识提供程序将 ID 令牌发送回 Azure AD B2C 后，Azure AD B2C 从令牌中的将声明映射到 Azure AD B2C 可识别和使用的声明。</span><span class="sxs-lookup"><span data-stu-id="d62f4-105">After the custom identity provider sends an ID token back to Azure AD B2C, Azure AD B2C maps the claims from a token to the claims that Azure AD B2C recognizes and uses.</span></span>

## <a name="properties"></a><span data-ttu-id="d62f4-106">属性</span><span class="sxs-lookup"><span data-stu-id="d62f4-106">Properties</span></span>
|<span data-ttu-id="d62f4-107">属性</span><span class="sxs-lookup"><span data-stu-id="d62f4-107">Property</span></span>|<span data-ttu-id="d62f4-108">类型</span><span class="sxs-lookup"><span data-stu-id="d62f4-108">Type</span></span>|<span data-ttu-id="d62f4-109">描述</span><span class="sxs-lookup"><span data-stu-id="d62f4-109">Description</span></span>|
|:-------|:---|:----------|
|<span data-ttu-id="d62f4-110">userId</span><span class="sxs-lookup"><span data-stu-id="d62f4-110">userId</span></span>|<span data-ttu-id="d62f4-111">字符串</span><span class="sxs-lookup"><span data-stu-id="d62f4-111">String</span></span>|<span data-ttu-id="d62f4-112">为已登录用户提供唯一标识符的声明。</span><span class="sxs-lookup"><span data-stu-id="d62f4-112">The claim that provides the unique identifier for the signed-in user.</span></span> <span data-ttu-id="d62f4-113">这是必需属性。</span><span class="sxs-lookup"><span data-stu-id="d62f4-113">It is a required propoerty.</span></span>|
|<span data-ttu-id="d62f4-114">displayName</span><span class="sxs-lookup"><span data-stu-id="d62f4-114">displayName</span></span>|<span data-ttu-id="d62f4-115">字符串</span><span class="sxs-lookup"><span data-stu-id="d62f4-115">String</span></span>|<span data-ttu-id="d62f4-116">为用户提供显示名称或全名的声明。</span><span class="sxs-lookup"><span data-stu-id="d62f4-116">The claim that provides the display name or full name for the user.</span></span> <span data-ttu-id="d62f4-117">这是必需属性。</span><span class="sxs-lookup"><span data-stu-id="d62f4-117">It is a required propoerty.</span></span>|
|<span data-ttu-id="d62f4-118">givenName</span><span class="sxs-lookup"><span data-stu-id="d62f4-118">givenName</span></span>|<span data-ttu-id="d62f4-119">字符串</span><span class="sxs-lookup"><span data-stu-id="d62f4-119">String</span></span>|<span data-ttu-id="d62f4-120">提供用户名字的声明。</span><span class="sxs-lookup"><span data-stu-id="d62f4-120">The claim that provides the first name of the user.</span></span>|
|<span data-ttu-id="d62f4-121">surname</span><span class="sxs-lookup"><span data-stu-id="d62f4-121">surname</span></span>|<span data-ttu-id="d62f4-122">字符串</span><span class="sxs-lookup"><span data-stu-id="d62f4-122">String</span></span>|<span data-ttu-id="d62f4-123">提供用户姓氏的声明。</span><span class="sxs-lookup"><span data-stu-id="d62f4-123">The claim that provides the last name of the user.</span></span>|
|<span data-ttu-id="d62f4-124">email</span><span class="sxs-lookup"><span data-stu-id="d62f4-124">email</span></span>|<span data-ttu-id="d62f4-125">字符串</span><span class="sxs-lookup"><span data-stu-id="d62f4-125">String</span></span>|<span data-ttu-id="d62f4-126">提供用户名电子邮件地址的声明。</span><span class="sxs-lookup"><span data-stu-id="d62f4-126">The claim that provides the email address of the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d62f4-127">关系</span><span class="sxs-lookup"><span data-stu-id="d62f4-127">Relationships</span></span>
<span data-ttu-id="d62f4-128">无。</span><span class="sxs-lookup"><span data-stu-id="d62f4-128">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d62f4-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d62f4-129">JSON representation</span></span>
<span data-ttu-id="d62f4-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d62f4-130">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.claimsMapping"
}
-->

``` json
{
  "userId": "String",
  "givenName": "String",
  "surname": "String",
  "email": "String",
  "displayName": "String"
  }
```


