---
title: riskUserActivity 资源类型
description: riskUserActivity 检测
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b8be06588194ad46722fc58b46c78e4a8bed53ec
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895914"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="81704-103">riskUserActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="81704-103">riskUserActivity resource type</span></span>

<span data-ttu-id="81704-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81704-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="81704-105">表示 azure AD 用户的风险活动，由 Azure AD Identity Protection 确定。</span><span class="sxs-lookup"><span data-stu-id="81704-105">Represents the risk activites of an Azure AD user as determined by Azure AD Identity Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="81704-106">属性</span><span class="sxs-lookup"><span data-stu-id="81704-106">Properties</span></span>
|<span data-ttu-id="81704-107">属性</span><span class="sxs-lookup"><span data-stu-id="81704-107">Property</span></span>|<span data-ttu-id="81704-108">类型</span><span class="sxs-lookup"><span data-stu-id="81704-108">Type</span></span>|<span data-ttu-id="81704-109">说明</span><span class="sxs-lookup"><span data-stu-id="81704-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81704-110">介绍</span><span class="sxs-lookup"><span data-stu-id="81704-110">detail</span></span>|<span data-ttu-id="81704-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="81704-111">riskDetail</span></span>|<span data-ttu-id="81704-112">检测到的风险的详细信息。</span><span class="sxs-lookup"><span data-stu-id="81704-112">Details of the detected risk.</span></span> <span data-ttu-id="81704-113">可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="81704-113">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="81704-114">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="81704-114">riskEventTypes</span></span>|<span data-ttu-id="81704-115">String collection</span><span class="sxs-lookup"><span data-stu-id="81704-115">String collection</span></span>|<span data-ttu-id="81704-116">检测到的风险事件的类型。</span><span class="sxs-lookup"><span data-stu-id="81704-116">The type of risk event detected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81704-117">关系</span><span class="sxs-lookup"><span data-stu-id="81704-117">Relationships</span></span>
<span data-ttu-id="81704-118">无。</span><span class="sxs-lookup"><span data-stu-id="81704-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="81704-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81704-119">JSON representation</span></span>
<span data-ttu-id="81704-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81704-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.riskUserActivity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskUserActivity",
  "riskEventTypes": [
    "String"
  ],
  "detail": "String"
}
```

