---
title: identityGovernance 资源类型
description: 用于包含标识管理资源的单一方法。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: be8bb2f562b05892f972431fd32db72b29af305a
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61649681"
---
# <a name="identitygovernance-resource-type"></a>identityGovernance 资源类型

命名空间：microsoft.graph

标识管理单一对象是以下标识Azure Active Directory通过以下资源和 API 公开的标识管理功能的容器：

+ [访问审查](accessreviewsv2-overview.md)
+ [权利管理](entitlementmanagement-overview.md)
+ [应用同意](consentrequests-overview.md)
+ [使用条款](agreement.md)

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|accessReviews|[accessReviewSet](accessreviewset.md)| 公开访问评审 API 和功能的基本资源的容器。 当前仅公开 [定义](accessreviewscheduledefinition.md) 资源。|
|appConsent|[appConsent](appconsentapprovalroute.md)| 公开应用许可请求 API 和功能的基本资源的容器。 当前仅公开 [appConsentRequests](appconsentrequest.md) 资源。|
|entitlementManagement|[entitlementManagement](entitlementmanagement.md)| 权利管理资源的容器，包括[accessPackageCatalog、connectedOrganization](accesspackagecatalog.md)和[entitlementManagementSettings](entitlementmanagementsettings.md)。 [](connectedorganization.md)|
|termsOfUse|[termsOfUseContainer](termsofusecontainer.md)| 公开使用条款 API 及其功能（包括协议和[agreementAcceptances）的资源容器](agreementacceptance.md)。 [](agreement.md) |

