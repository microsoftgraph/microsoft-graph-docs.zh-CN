---
title: 多租户管理枚举值
description: Microsoft Graph多租户管理枚举值
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: enumTypes
ms.openlocfilehash: 9b93794e763025b409ff00c0a2b5d13909ca705d
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095949"
---
# <a name="multi-tenant-management-enumeration-values"></a>多租户管理枚举值

### <a name="delegatedprivilegestatus-values"></a>delegatedPrivilegeStatus 值

|Member|
|:---|
|无|
|delegatedAdminPrivileges|
|unknownFutureValue|
|granularDelegatedAdminPrivileges|
|delegatedAndGranularDelegetedAdminPrivileges|

### <a name="managementactionstatus-values"></a>managementActionStatus 值

|Member|
|:---|
|toAddress|
|完成|
|error|
|超时|
|inProgress|
|计划|
|resolvedBy3rdParty|
|resolvedThroughAlternateMitigation|
|riskAccepted|
|unknownFutureValue|

### <a name="managementcategory-values"></a>managementCategory 值

|Member|
|:---|
|自 定义|
|设备|
|身份|
|unknownFutureValue|

### <a name="managementparametervaluetype-values"></a>managementParameterValueType 值

|Member|
|:---|
|string|
|integer|
|boolean|
|guid|
|stringCollection|
|integerCollection|
|booleanCollection|
|guidCollection|
|unknownFutureValue|

### <a name="tenantonboardingstatus-values"></a>tenantOnboardingStatus 值

|Member|
|:---|
|资格|
|inProcess|
|积极|
|无效|
|unknownFutureValue|

### <a name="tenantonboardingeligibilityreason-values"></a>tenantOnboardingEligibilityReason 值

|Member|
|:---|
|无|
|contractType|
|delegatedAdminPrivileges|
|usersCount|
|license|
|unknownFutureValue|

### <a name="workloadactioncategory-values"></a>workloadActionCategory 值

|Member|
|:---|
|自动化|
|手动|
|unknownFutureValue|

### <a name="workloadactionstatus-values"></a>workloadActionStatus 值

|Member|
|:---|
|toAddress|
|完成|
|error|
|超时|
|inProgress|
|unknownFutureValue|

### <a name="workloadonboardingstatus-values"></a>workloadOnboardingStatus 值

|Member|
|:---|
|notOnboarded|
|载入|
|unknownFutureValue|
