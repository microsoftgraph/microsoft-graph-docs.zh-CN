---
title: 枚举值
description: Microsoft Graph 枚举值
ms.openlocfilehash: 2f8bd0065136077cda2228cbec1c2d34d546c7d1
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542802"
---
### <a name="contactrelationship-values"></a>contactRelationship 值

|Member|值|说明|
|:---|:---|:---|
|母语|0|用户的父级。|
|彼此|1| 用户的相对路径。|
|aide|2 | 用户的 aide。|
|dr。|3 | 用户的医生。|
|监护|4 | 用户的监护人。|
|该子|5 | 用户的子级。|
|相互|6 | 与用户的未指定关系。|
|向 unknownfuturevalue|7 | 用于将来兼容性的标记值。|

### <a name="timezonestandard-values"></a>timeZoneStandard 值

| 值
|:-----------------
| 时间
| iana


### <a name="freebusystatus-values"></a>freeBusyStatus 值

| Member            |值
|:------------------|:-------
| 任意              | 0
| 暂         | 1
| 空闲              | 2 
| oof               | 3 
| workingElsewhere  | 4 
| unknown           | -1


### <a name="physicaladdresstype-values"></a>: physicaladdresstype 值

| 值
|:-------------------------
| unknown 
| 回收
| 知情 
| 相互


### <a name="attendeetype-values"></a>attendeeType 值

| 值
|:-------------------------
| 必需
| 可选
| 资源


### <a name="externalaudiencescope-values"></a>externalAudienceScope 值

| 值
|:-------------------------
| 无
| contactsOnly
| 各种


### <a name="automaticrepliesstatus-values"></a>automaticRepliesStatus 值

| 值
|:-------------------------
| 禁用
| alwaysenabled 启用
| 已计划


### <a name="calendarcolor-values"></a>calendarColor 值

| Member     | 值
|:-----------|:----------
| 自动       | -1
| lightBlue  | 0
| lightGreen | 1
| lightOrange| 2 
| lightGray  | 3 
| lightYellow| 4 
| lightTeal  | 5 
| lightPink  | 6 
| lightBrown | 7 
| lightRed   | 8 
| maxColor   | 9 


### <a name="educationsynchronizationprofilestate-values"></a>educationSynchronizationProfileState 值

| Member     | 值
|:-----------|:----------
| 删除          | 2 
| deletionFailed    | 3 
| provisioningFailed | 5 
| 已设置        | 6 
| 设置       | 7 
| 向 unknownfuturevalue | 8 


### <a name="educationsynchronizationstatus-values"></a>educationSynchronizationStatus 值

| Member     | 值
|:-----------|:----------
| 停留          | 0
| inProgress    | 1
| success | 2 
| error        | 3 
| validationError | 4 
| 隔离       | 5 
| 向 unknownfuturevalue | 6 

### <a name="educationexternalsource-values"></a>educationExternalSource 值

| 值
|:-------------------------
| sis
| 手动
| 向 unknownfuturevalue


### <a name="educationgender-values"></a>educationGender 值

| 值
|:-------------------------
| 接头
| 触点
| 相互
| 向 unknownfuturevalue


### <a name="eventtype-values"></a>事件的值

| 值
|:-------------------------
| singleInstance
| 重复
| 异常
| seriesMaster


### <a name="sensitivity-values"></a>敏感度值

| 值
|:-------------------------
| 通用
| personal
| private
| 秘密


### <a name="importance-values"></a>重要性值

| 值
|:-------------------------
| 降低
| 通用
| 高效


### <a name="educationuserrole-values"></a>educationUserRole 值
| 值
|:---------------------
| student
| teacher
| 无
| 向 unknownfuturevalue


### <a name="meetingmessagetype-values"></a>meetingMessageType 值

| 值
|:-----------------
| 无
| meetingRequest
| meetingCancelled
| meetingAccepted
| meetingTentativelyAccepted
| meetingDeclined


### <a name="followupflagstatus-values"></a>followupFlagStatus 值

| 值
|:-------------------------
| notFlagged
| complete
| 带


### <a name="inferenceclassificationtype-values"></a>inferenceClassificationType 值

| 值
|:-----------------
| 介绍
| 相互


### <a name="iosnotificationalerttype-values"></a>iosNotificationAlertType 值

| 值
|:-------------------------
| deviceDefault
| 分隔
| 适合
| 无

### <a name="deviceenrollmentfailurereason-values"></a>deviceEnrollmentFailureReason 值

| 值
|:-------------
| unknown
| authentication
| 批准
| accountValidation
| userValidation
| deviceNotSupported
| inMaintenance
| badRequest
| featureNotSupported
| enrollmentRestrictionsEnforced
| clientDisconnected


### <a name="bodytype-values"></a>office.mailboxenums.bodytype 值
| 值
|:---------
| text
| Html


### <a name="locationtype-values"></a>locationType 值

| 值
|:-------------------------
| 设置
| conferenceRoom
| homeAddress
| businessAddress
| geoCoordinates
| streetAddress
| 住
| 餐馆
| localBusiness
| postalAddress

### <a name="locationuniqueidtype-values"></a>locationUniqueIdType 值

| 值
|:-------------------------
| unknown
| locationStore
| 文件夹
| private
| 必应


### <a name="messageactionflag-values"></a>messageActionFlag 值

| 值
|:-------------------------
| 任意
| call
| doNotForward
| 努力
| 仅供参考
| 转发
| noResponseNecessary
| 自述
| 回复
| replyToAll
| 概述


### <a name="onenoteuserrole-values"></a>onenoteUserRole 值

| Member      | 值
|:------------|:------------
| Owner       | 0
| 参与者 | 1
| 读者      | 2 
| 无        | -1


### <a name="operationstatus-values"></a>operationStatus 值

| 值
|:-----------------
| NotStarted
| 运行
| Completed
| Failed


### <a name="onenotepatchactiontype-values"></a>onenotePatchActionType 值

| 值
|:-------------------------
| Replace
| Append
| 删除
| Insert
| 计算

### <a name="onenotepatchinsertposition-values"></a>onenotePatchInsertPosition 值

| 值
|:-------------------------
| 段后
| Before


### <a name="phonetype-values"></a>phoneType 值

| 值
|:-------------------------
| 回收
| 知情
| 流动
| 相互
| 协助
| homeFax
| businessFax
| otherFax
| pager
| 无线电台


### <a name="plannerpreviewtype-values"></a>plannerPreviewType 值

| 值
|:-------------------------
| 自动
| noPreview
| checklist
| description
| reference


### <a name="status-values"></a>status 值

| 值
|:-----------------
| 工作
| updated
| deleted
| 忽视
| 向 unknownfuturevalue


### <a name="weekindex-values"></a>weekIndex 值

| 值
|:-------------------------
| 前
| 第二个
| 次
| 四分之一
| 末


### <a name="dayofweek-values"></a>dayOfWeek 值

| 值
|:-------------------------
| 日
| 星期一
| 2001
| 星期三
| 星期三
| 之前
| 星期六

### <a name="recurrencepatterntype-values"></a>recurrencePatternType 值

| 值
|:-------------------------
| 每日
| 周历
| absoluteMonthly
| relativeMonthly
| absoluteYearly
| relativeYearly


### <a name="recurrencerangetype-values"></a>recurrenceRangeType 值

| 值
|:-------------------------
| endDate
| noEnd
| 数字化


### <a name="onenotesourceservice-values"></a>onenoteSourceService 值
| 值
|:---------------------
| 未知
| OneDrive
| OneDriveForBusiness
| OnPremOneDriveForBusiness


### <a name="responsetype-values"></a>responseType 值

| 值
|:-------------------------
| 无
| 组织者
| tentativelyAccepted
| 接受
| 邀请
| notResponded


### <a name="activitydomain-values"></a>activityDomain 值

| 值
|:-------------------------
| unknown
| 工时
| personal
| unrestricted


### <a name="websitetype-values"></a>websiteType 值

| 值
|:-------------------------
| 相互
| 回收
| 工时
| 博客
| profile


### <a name="categorycolor-values"></a>categoryColor 值

| Member   |值    
|:---------|:--------
| 无     | -1      
| preset0  | 0       
| preset1  | 1       
| preset2  | 2        
| preset3  | 3        
| preset4  | 4        
| preset5  | 5        
| preset6  | 6        
| preset7  | 7        
| preset8  | 8        
| preset9  | 9        
| preset10 | 10       
| preset11 | 11       
| preset12 | 12       
| preset13 | 13       
| preset14 | 14       
| preset15 | 15       
| preset16 | 16       
| preset17 | ×      
| preset18 | 18      
| preset19 | 合      
| preset20 | 20      
| preset21 | 不足      
| preset22 | 22      
| preset23 | 上午      
| preset24 | 24      

### <a name="alertfeedback-values"></a>alertFeedback 值

由分析师提供的警报上可能的反馈值。

|Member|值|说明|
|:---|:---|:---|
|unknown|0|陌生.|
|truePositive|1|警报为 true-肯定。|
|falsePositive|2 | 警报为 false-肯定。|
|benignPositive|3 | 警报为良性-肯定。|

### <a name="filehashtype-values"></a>fileHashType 值

|Member|值|说明|
|:---|:---|:---|
|unknown|0|未知类型。|
|sha1|1|SHA1 哈希类型。|
|sha256|2 | SHA256 哈希类型。|
|md5|3 | MD5 哈希类型。|
|authenticodeHash256|4 | AuthenticodeHash256 哈希类型。|
|lsHash|5 | LsHash 哈希类型。|
|ctph|6 | CTPH 哈希类型。|
|peSha1|7 | PESHA1 哈希类型。|
|peSha256|8 | PESHA256 哈希类型。|

### <a name="connectiondirection-values"></a>connectionDirection 值

|Member|值|说明|
|:---|:---|:---|
|unknown|0|未知的连接。|
|进货|1|入站连接。|
|出站|2 | 出站连接。|

### <a name="connectionstatus-values"></a>connectionStatus 值

|Member|值|说明|
|:---|:---|:---|
|unknown|0|未知的连接状态。|
|尝试|1|已尝试连接。|
|完成|2 | 连接成功。|
|堵塞|3 | 连接被阻止。|
|未能|4 | 连接失败。|

### <a name="processintegritylevel-values"></a>processIntegrityLevel 值

|Member|值|说明|
|:---|:---|:---|
|unknown|0|陌生.|
|可信|10 |完整性级别不受信任。|
|降低|20| 完整性级别较低。|
|中等|30| 完整性级别为 "中"。|
|高效|40| 完整性级别为 "高"。|
|system|50| 完整性级别为 "系统"。|

### <a name="registryhive-values"></a>registryHive 值

由定义的[https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives)注册表配置单元的枚举。

|Member|值|说明|
|:---|:---|:---|
|unknown|0|未知配置单元。|
|currentConfig|1|HKEY_CURRENT_CONFIG 配置单元。|
|currentUser|2 | HKEY_CURRENT_USER 配置单元。|
|localMachineSam|3 | HKEY_LOCAL_MACHINE\SAM 配置单元。|
|localMachineSamSoftware|4 | HKEY_LOCAL_MACHINE\Software 配置单元。|
|localMachineSystem|5 | HKEY_LOCAL_MACHINE\System 配置单元。|
|usersDefault|6 | HKEY_USERS\\。默认配置单元。|

### <a name="registryoperation-values"></a>registryOperation 值

更改注册表项名称和/或值的操作。

|Member|值|说明|
|:---|:---|:---|
|unknown|0|未知的注册表值类型。|
|create|1|创建注册表。|
|modify|2 |修改注册表。|
|delete|3 |删除注册表。|

### <a name="registryvaluetype-values"></a>registryValueType 值

由定义的[https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types)注册表值类型的枚举。

|Member|值|说明|
|:---|:---|:---|
|unknown|0|未知的注册表值类型。|
|数字|1|REG_BINARY 注册表值类型。|
|值|2 | REG_DWORD 注册表值类型。|
|dwordLittleEndian|3 | REG_DWORD_LITTLE_ENDIAN 注册表值类型。|
|dwordBigEndian|4 | REG_DWORD_BIG_ENDIAN 注册表值类型。|
|expandSz|5 | REG_EXPAND_SZ 注册表值类型。|
|link|6 | REG_LINK 注册表值类型。|
|multiSz|7 | REG_MULTI_SZ 注册表值类型。|
|无|8 | REG_NONE 注册表值类型。|
|qword|9 | REG_QWORD 注册表值类型。|
|qwordlittleEndian|10 | REG_QWORD_LITTLE_ENDIAN 注册表值类型。|
|sz|11 | REG_SZ 注册表值类型。|

### <a name="alertseverity-values"></a>alertSeverity 值

警报严重性的枚举。

|Member|值|说明|
|:---|:---|:---|
|unknown|0|严重度未知。|
|之|1|严重性仅适用于信息。|
|降低|2 | 严重性为低。|
|中等|3 | 严重性为 "中"。|
|高效|4 | 严重性为高。|

### <a name="alertstatus-values"></a>alertStatus 值

警报生命周期状态 (阶段) 的可能值。

|Member|值|说明|
|:---|:---|:---|
|unknown|0|未知状态。|
|newAlert|10 | 警报是新的。|
|inProgress|20|警报正在进行中。|
|经过|30|警报已解决。|

### <a name="emailrole-values"></a>emailRole 值

电子邮件角色的可能值。

|Member|值|说明|
|:---|:---|:---|
|unknown|0|未知角色。|
|sender|1|电子邮件的发件人。|
|recipient|2 |电子邮件的收件人。|

### <a name="logontype-values"></a>logonType 值

用户登录方法的可能值。

|Member|值|说明|
|:---|:---|:---|
|unknown|-1|陌生.|
|式|0|登录是交互式的。|
|remoteInteractive|1| 登录是远程交互的。|
|network|2 | 登录为网络。|
|batch|3 | 登录是批处理。|
|service|4 | 登录为 "服务"。|

### <a name="useraccountsecuritytype-values"></a>userAccountSecurityType 值

每个 Windows 定义的用户帐户类型 (组成员身份) 可能的值。

|Member|值|说明|
|:---|:---|:---|
|unknown|-1|陌生.|
|普通|0|"标准用户" 组的成员。|
|能力|1| Power Users 组的成员。|
|联系|2 | Administrators 组的成员。|
